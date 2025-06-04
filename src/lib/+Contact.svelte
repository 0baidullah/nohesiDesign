<script lang="ts">
  import { enhance } from "$app/forms";
  import { fade } from "svelte/transition";
  import { writable } from "svelte/store";
  //   import DarkStrip from './DarkStrip.svelte';

  // Form schema using Svelte's reactive declarations
  let name = "";
  let email = "";
  let question = "";

  let success = writable<string | null>(null);
  let serverError = writable<string | null>(null);
  let isPending = writable(false);

  // Character counter
  $: questionLength = question.length;

  // Validation functions
  const validateName = () => {
    if (!name) return "Name is required";
    return "";
  };

  const validateEmail = () => {
    if (!email) return "Email is required";
    if (!/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email))
      return "Invalid email address";
    return "";
  };

  const validateQuestion = () => {
    if (!question) return "Question is required";
    if (question.length > 400)
      return "Question must be less than 400 characters";
    return "";
  };

  // Combined validation
  $: nameError = validateName();
  $: emailError = validateEmail();
  $: questionError = validateQuestion();
  $: formValid = !nameError && !emailError && !questionError;

  async function handleSubmit() {
    $isPending = true;
    $serverError = null;
    $success = null;

    try {
      const res = await fetch("/api/contactForm", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({ name, email, question }),
      });

      if (!res.ok) {
        const errorData = await res.json();
        throw errorData;
      }

      $success = "Your question has been submitted!";
      name = "";
      email = "";
      question = "";
    } catch (error: any) {
      const errObj =
        typeof error === "object" && error !== null
          ? (error as Record<string, any>)
          : {};
      $serverError =
        errObj.error?.name?.[0] ||
        errObj.error?.email?.[0] ||
        errObj.error?.question?.[0] ||
        "Something went wrong.";
    } finally {
      $isPending = false;
    }
  }
</script>

<div class="bg-gray-1000 text-white py-20 px-6 md:px-12  mx-10">
  <div
    class="max-w-7xl mx-auto flex flex-col lg:flex-row items-start justify-between gap-10"
  >
    <div class="flex-1 text-left">
      <h1
        class="text-4xl md:text-5xl lg:text-6xl font-extrabold leading-tight text-gray-300 uppercase"
      >
        Questions?
        <br />
        <span class="text-white">No Problem,</span>
        <br />
        <span class="text-white">
          We Have The <span class="text-gray-300">Answers.</span>
        </span>
      </h1>
    </div>

    <form
      use:enhance={handleSubmit}
      class="flex-1 w-full bg-[#0f0f0f] border border-gray-700 rounded-xl p-6 space-y-4"
    >
      <div
        class="bg-yellow-500/20 border border-yellow-500 text-yellow-400 text-sm p-3 rounded"
      >
        ⚠️ We may take up to 24–78 hours to reply
      </div>

      {#if $serverError}
        <div
          transition:fade
          class="text-red-400 text-sm bg-red-400/10 border border-red-400 p-2 rounded"
        >
          {$serverError}
        </div>
      {/if}

      {#if $success}
        <div
          transition:fade
          class="text-green-400 text-sm bg-green-400/10 border border-green-400 p-2 rounded"
        >
          {$success}
        </div>
      {/if}

      <div>
        <!-- svelte-ignore a11y_label_has_associated_control -->
        <label class="block text-sm mb-1">Name</label>
        <input
          type="text"
          bind:value={name}
          placeholder="John Doe"
          class="w-full bg-black border border-gray-700 rounded px-3 py-2 text-sm focus:outline-none focus:ring-2 focus:ring-purple-500"
        />
        {#if nameError}
          <p class="text-red-500 text-xs mt-1">{nameError}</p>
        {/if}
      </div>

      <div>
        <!-- svelte-ignore a11y_label_has_associated_control -->
        <label class="block text-sm mb-1">Email</label>
        <input
          type="email"
          bind:value={email}
          placeholder="example@mail.com"
          class="w-full bg-black border border-gray-700 rounded px-3 py-2 text-sm focus:outline-none focus:ring-2 focus:ring-purple-500"
        />
        {#if emailError}
          <p class="text-red-500 text-xs mt-1">{emailError}</p>
        {/if}
      </div>

      <div>
        <!-- svelte-ignore a11y_label_has_associated_control -->
        <label class="block text-sm mb-1">Your question</label>
        <!-- svelte-ignore element_invalid_self_closing_tag -->
        <textarea
          maxlength={400}
          bind:value={question}
          placeholder="..."
          class="w-full bg-black border border-gray-700 rounded px-3 py-2 text-sm focus:outline-none focus:ring-2 focus:ring-purple-500"
        />
        {#if questionError}
          <p class="text-red-500 text-xs mt-1">{questionError}</p>
        {/if}
        <div class="text-right text-xs text-gray-500">{questionLength}/400</div>
      </div>

      <div class="mt-4">
        <div class="bg-purple-400 rounded p-4 w-fit text-black text-sm">
          [reCAPTCHA goes here]
        </div>
      </div>

      <button
        type="submit"
        disabled={!formValid || $isPending}
        class="w-full bg-purple-600 hover:bg-purple-700 text-white font-bold py-2 rounded-lg uppercase tracking-wide mt-4 transition disabled:opacity-50"
      >
        {$isPending ? "Sending..." : "Send"}
      </button>
    </form>
  </div>
</div>

<style>
  .bg-gray-1000 {
    background-color: #111;
  }
  input,
  textarea {
    transition:
      border-color 0.2s ease,
      box-shadow 0.2s ease;
  }
  button {
    transition:
      background-color 0.2s ease,
      opacity 0.2s ease;
  }
</style>
