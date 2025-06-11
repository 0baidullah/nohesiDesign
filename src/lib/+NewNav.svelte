<script>
  let menuOpen = false;
  import logo from "../lib/assets/black.png";
  import Arrow from "../lib/assets/Right Arrow.png";
</script>

<nav
  class="bg-white text-black w-full flex items-center justify-between h-20 lg:gap-12 lg:py-5
   lg:px-12 sm:px-4 px-2 relative"
>
  <div class="lg:hidden flex items-center justify-items-center ">
    <a href="/" class="flex items-center group">
      <img
        src={logo}
        alt="Logo"
        class="lg:h-8 lg:w-8 sm:h-8 sm:w-8 rounded-full"
      />
    </a>
  </div>
  <ul
    class="absolute w-full top-14 left-0  flex flex-col lg:flex-row gap-10 lg:gap-12 items-center font-['Roboto_Flex'] text-[15px] leading-5 lg:static
    lowercase  lg:flex "
    class:hidden={!menuOpen}
    >
    <li>
      <div class="  items-center">
        <a href="/" class="flex items-center group">
          <img
            src={logo}
            alt="Logo"
            class=" hidden lg:flex lg:h-8 lg:w-8 rounded-full"
          />
        </a>
      </div>
    </li>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
    <li><a href="/services">Services</a></li>
    <li><a href="/contact">Contact</a></li>
    <li><a href="/subscription">Subscription</a></li>
    <div class="lg:hidden px-3 w-full flex flex-col gap-2 items-center">
      <button
        class="w-full font-['Roboto_Flex'] text-sm whitespace-nowrap h-[40px] border-gray-300 rounded-2xl"
        style="background:#F0F0F0"
      >
        Sign in
      </button>

      <button
        class="w-full font-['Roboto_Flex'] text-sm whitespace-nowrap h-[40px] border-blue-700 rounded-2xl"
        style="background: var(--def, #5C53E9);">Sign Up</button
      >
    </div>
  </ul>
  <button
    type="button"
    aria-label="Toggle menu"
    on:click={() => (menuOpen = !menuOpen)}
    class="lg:hidden"
  >
    <i class="fa-solid fa-bars text-black"></i>
  </button>
  <div class="hidden lg:flex w-50% gap-2">
    <button
      class="font-['Roboto_Flex'] text-[15px] whitespace-nowrap w-[92px] h-[40px] border-gray-300 rounded-2xl"
      style="background:#F0F0F0">sign in</button
    >
    <button
      class="font-['Roboto_Flex'] text-[15px] whitespace-nowrap w-[92px] h-[40px] border-blue-700 rounded-2xl"
      style="background: var(--def, #5C53E9);">sign up</button
    >
  </div>
</nav>
