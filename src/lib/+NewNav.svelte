





    <script>
  let menuOpen = false;
</script>

<nav class="bg-white text-black mt-4 flex items-center justify-between h-10 lg:gap-12 px-6 mx-auto">
  <div></div>
  <ul
    class="absolute top-16 w-full flex flex-col gap-6 mt-5 items-center font-['Roboto_Flex'] text-[15px] lg:items-center lg:font-medium leading-5 tracking-normal text-center lg:static
    lg:flex-row lg:space-x-6 font-bold uppercase lg:text-xs lg:gap-12 lg:flex"
    class:hidden={!menuOpen}
  >
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
    <li><a href="/services">Services</a></li>
    <li><a href="/contact">Contact</a></li>
    <li><a href="/subscription">Subscription</a></li>
    <div class="lg:hidden px-3 w-full flex flex-col gap-2 items-center space-x-2">
      <button class="w-full font-['Roboto_Flex'] text-sm whitespace-nowrap h-[40px] border-gray-300 rounded-2xl" style="background:#F0F0F0">Sign in</button>
      <button class="w-full font-['Roboto_Flex'] text-sm whitespace-nowrap h-[40px] border-blue-700 rounded-2xl" style="background: var(--def, #5C53E9);">Sign Up</button>
    </div>
  </ul>
  <button type="button" aria-label="Toggle menu" on:click={() => menuOpen = !menuOpen} class="lg:hidden">
    <i class="fa-solid fa-bars text-black"></i>
  </button>
  <div class="hidden lg:flex lg:items-center space-x-2 my-15">
    <button class="font-['Roboto_Flex'] text-sm whitespace-nowrap w-[92px] h-[40px] border-gray-300 rounded-2xl" style="background:#F0F0F0">Sign in</button>
    <button class="font-['Roboto_Flex'] text-sm whitespace-nowrap w-[92px] h-[40px] border-blue-700 rounded-2xl" style="background: var(--def, #5C53E9);">Sign Up</button>
  </div>
</nav>