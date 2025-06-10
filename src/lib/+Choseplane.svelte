




<script>
  // Same script logic
  import { onMount } from "svelte";

  let selectedPlan = "annually";
  let memberCount = 28643;
  /**
   * @type {any[]}
   */
  let digits = [];

  onMount(() => {
    digits = memberCount.toString().split("");
  });
</script>

<!-- Responsive Container -->
<div class="w-full px-4 py-8" style="background: #08060A;">
  <div class="relative mx-auto max-w-[1368px] px-4">
    <!-- Background Patterns -->
    <div class="absolute inset-0 opacity-10">
      <div class="absolute top-0 left-0 w-full h-full bg-gradient-to-r from-transparent via-blue-500/20 to-transparent"></div>
      <div class="absolute top-1/2 left-1/4 w-32 h-32 bg-pink-500/10 rounded-full blur-xl"></div>
      <div class="absolute bottom-1/4 right-1/4 w-24 h-24 bg-blue-500/10 rounded-full blur-xl"></div>
    </div>

    <!-- Foreground Content -->
    <div
      class="relative z-10 flex flex-wrap justify-center items-center gap-4 text-center"
    >
      <!-- Join -->
      <h1
        class="font-['Roboto_Flex'] font-extrabold text-4xl sm:text-5xl md:text-6xl lg:text-[64px] uppercase text-white"
      >
        Join
      </h1>

      <!-- Roller Digits -->
      <div class="flex gap-[2px]">
        {#each digits as digit, i}
          <div class="roller">
            <div
              class="roller-digit"
              style="transform: translateY(-{digit * 3.5}rem); animation-delay: {i * 0.1}s"
            >
              {#each Array(10) as _, j}
                <div class="digit-row">{j}</div>
              {/each}
            </div>
          </div>
        {/each}
      </div>

      <!-- OTHERS -->
      <!-- <h1
        class="font-['Roboto_Flex'] font-extrabold text-4xl sm:text-5xl md:text-6xl lg:text-[64px] uppercase text-white"
      >
        OTHERS
      </h1> -->
    </div>
  </div>
</div>

<style>
  .roller {
    overflow: hidden;
    height: 4rem;
    width: 3rem;
    display: inline-block;
    position: relative;
    border-radius: 0.25rem;
  }

  .roller-digit {
    display: flex;
    flex-direction: column;
    position: absolute;
    animation: rollDownBounce 1.2s ease-out forwards;
  }

  .digit-row {
    height: 3.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 64px;
    color: #DD0355;
    font-weight: 1000;
  }

  @keyframes rollDownBounce {
    0% {
      transform: translateY(-100%);
    }
    85% {
      transform: translateY(calc(var(--target-translate, 0) + 0.1rem));
    }
    100% {
      /* Handled inline */
    }
  }
</style>
