<script>
  //   import { page } from '$app/stores';
  import { fade, slide } from "svelte/transition";
  import logo from "../lib/assets/NO HESI.svg";
  import logo2 from "../lib/assets/Vector.png";
  import Alert from "../lib/assets/Ellipse 1.png";
  import Star from "../lib/assets/Star.svg";
  import Data from "../lib/assets/Database.png";
  import File from "../lib/assets/FileArrowDown.svg";
  import Bell from "../lib/assets/Bell.png";
  import Avatar from "../lib/assets/9fbd4972fc0c3ffddfc14a8b901a6aa53a99193c.jpg";
  import Arrow from "../lib/assets/Arrow.png";
  
  let isOpen = false;
  let isMobileMenuOpen = false;

  const toggleMobileMenu = () => {
    isMobileMenuOpen = !isMobileMenuOpen;
  };

  const closeMobileMenu = () => {
    isMobileMenuOpen = false;
  };
</script>

<nav
  class="absolute  h-[60px] w-full  top-5  flex px-2 py-3 justify-between items-center rounded-2xl border border-white/5 bg-[rgba(8,6,10,0.83)] backdrop-blur-xl"
>
  <div class="flex justify-between items-center">
    <!-- Logo Section - Exactly as original -->
    <div class="w-32 h-11 gap-1" style="background: #141216;">
      <a href="/" class="flex items-center px-4 py-2 rounded text-white">
        <img src={logo2} alt="Logo" class="w-4 h-4 mr-2 top-2" />
        <img src={logo} alt="Logo" class="w-20 h-7 top-2 left-6" />
      </a>
    </div>

    <!-- Desktop Navigation Links - Show on XL and above (1280px+) -->
    <div class="hidden xl:flex items-center w-full h-9 gap-2">
      <a href="/get-started">
        <button
          class="w-[90px] h-[36px] gap-1 rounded-md p-2 text-[14px] font-inter-tight font-medium leading-5 tracking-normal hover:bg-white/5 transition-colors"
        >
          Get started
        </button>
      </a>
      <a href="/get-started">
        <button
          class="w-[49px] h-[36px] gap-1 rounded-md p-2 text-[14px] font-medium leading-5 font-['Inter_Tight'] tracking-normal hover:bg-white/5 transition-colors"
        >
          Shop
        </button>
      </a>
      <a href="/get-started">
        <button
          class="w-[72px] h-[36px] gap-1 rounded-md p-2 text-[14px] font-medium leading-5 font-['Inter_Tight'] tracking-normal hover:bg-white/5 transition-colors"
        >
          About us
        </button>
      </a>
      <a href="/get-started">
        <button
          class="w-[52px] h-[36px] gap-1 rounded-md p-2 text-[14px] font-medium leading-5 font-['Inter_Tight'] tracking-normal hover:bg-white/5 transition-colors"
        >
          News
        </button>
      </a>
      <a href="/get-started">
        <button
          class="w-[73px] h-[36px] gap-1 rounded-md p-2 text-[14px] font-medium leading-5 font-['Inter_Tight'] tracking-normal hover:bg-white/5 transition-colors"
        >
          Contacts
        </button>
      </a>
      <a href="/get-started">
        <button
          class="w-[42px] h-[36px] gap-1 rounded-md p-2 text-[14px] font-medium leading-5 font-['Inter_Tight'] tracking-normal hover:bg-white/5 transition-colors"
        >
          FAQs
        </button>
      </a>
    </div>

    <!-- Compact Navigation Links for LG screens (1024px-1279px) -->
    <div class="hidden lg:flex xl:hidden items-center gap-1">
      <a href="/get-started">
        <button class="px-3 py-2 text-sm font-medium hover:bg-white/5 transition-colors rounded-md">
          Start
        </button>
      </a>
      <a href="/get-started">
        <button class="px-3 py-2 text-sm font-medium hover:bg-white/5 transition-colors rounded-md">
          Shop
        </button>
      </a>
      <a href="/get-started">
        <button class="px-3 py-2 text-sm font-medium hover:bg-white/5 transition-colors rounded-md">
          About
        </button>
      </a>
      <a href="/get-started">
        <button class="px-3 py-2 text-sm font-medium hover:bg-white/5 transition-colors rounded-md">
          News
        </button>
      </a>
    </div>
  </div>

  <div class="flex items-center">
    <!-- Desktop Action Buttons - Show on XL and above -->
    <div class="hidden xl:flex items-center h-9 gap-1">
      <a href="/get-started">
        <button
          class="w-[73px] h-9 flex items-center rounded-md px-3 py-2 border border-white/5 text-[14px] font-inter-tight font-medium leading-5 tracking-normal hover:bg-white/5 transition-colors"
        >
          <img src={Alert} alt="Alert Icon" class="w-4 h-4 mr-2" />
          <span
            class="w-[25px] h-[20px] text-[13px] font-inter-tight font-medium leading-5 tracking-normal"
            >Live</span
          >
        </button>
      </a>

      <a href="/Subscription">
        <button
          class="w-[133px] h-9 flex items-center rounded-md px-3 py-2 border border-white/5 text-[14px] font-inter-tight font-medium leading-5 tracking-normal hover:bg-white/5 transition-colors"
        >
          <img src={Star} alt="Alert Icon" class="w-4 h-4 mr-2" />
          <span
            class="w-[85px] h-[20px] text-[13px] font-inter-tight font-medium leading-5 tracking-normal"
            >Subscription</span
          >
        </button>
      </a>

      <a href="/get-started">
        <button
          class="w-[96px] h-9 flex items-center rounded-md px-3 py-2 border border-white/5 text-[14px] font-inter-tight font-medium leading-5 tracking-normal hover:bg-white/10 transition-colors"
          style="background: #252327;"
        >
          <img src={Data} alt="Alert Icon" class="w-4 h-4 mr-2" />
          <span
            class="w-[48px] h-[20px] text-[14px] font-inter-tight font-medium leading-5 tracking-normal"
            >Servers</span
          >
        </button>
      </a>

      <a href="/get-started">
        <button
          class="w-[167px] h-9 flex items-center rounded-md px-3 py-2 border border-white/5 text-[14px] font-inter-tight font-medium leading-5 tracking-normal hover:bg-white/5 transition-colors"
        >
          <img src={File} alt="Alert Icon" class="w-4 h-4 mr-2" />
          <span
            class="w-[120px] h-5 text-[13px] font-inter-tight font-medium leading-5 tracking-normal"
            >Download launcher</span
          >
        </button>
      </a>

      <a href="/get-started">
        <button
          class="w-[36px] h-9 flex items-center rounded-md px-2 py-2 border border-white/5 text-[14px] font-inter-tight font-medium leading-5 tracking-normal hover:bg-white/5 transition-colors"
        >
          <img src={Bell} alt="Alert Icon" class="w-4 h-4" />
        </button>
      </a>

      <div
        class="w-[160px] px-3 py-2 gap-[6px] ml-1 h-[36px] flex items-center bg-purple-800 rounded-md"
      >
        <img
          src={Avatar}
          alt="User Avatar"
          class="w-[28px] h-[28px] rounded-full border border-white/5"
        />
         <span
          class="w-[80px] h-[20px] text-[14px] font-inter-tight font-medium leading-5 tracking-normal text-white"
          >JohnDoe_911</span
        >
        <img src={Arrow} alt="Logo" class="w-[12px] h-[6px] ml-1" />
      </div> 
    </div>

    <!-- Compact Action Buttons for LG screens (1024px-1279px) -->
    <div class="hidden lg:flex xl:hidden items-center gap-1">
      <button class="p-2 border border-white/5 rounded-md hover:bg-white/5 transition-colors">
        <img src={Alert} alt="Live" class="w-4 h-4" />
      </button>
      <button class="p-2 border border-white/5 rounded-md hover:bg-white/5 transition-colors">
        <img src={Star} alt="Subscription" class="w-4 h-4" />
      </button>
      <button class="p-2 border border-white/5 rounded-md hover:bg-white/10 transition-colors bg-[#252327]">
        <img src={Data} alt="Servers" class="w-4 h-4" />
      </button>
      <button class="p-2 border border-white/5 rounded-md hover:bg-white/5 transition-colors">
        <img src={File} alt="Download" class="w-4 h-4" />
      </button>
      <button class="p-2 border border-white/5 rounded-md hover:bg-white/5 transition-colors">
        <img src={Bell} alt="Notifications" class="w-4 h-4" />
      </button>
      <div class="flex items-center bg-purple-800 rounded-md px-2 py-1 ml-1">
        <img src={Avatar} alt="User Avatar" class="w-6 h-6 rounded-full border border-white/5 mr-2" />
        <span class="text-sm font-medium text-white hidden lg:block xl:hidden">John</span>
        <img src={Arrow} alt="Arrow" class="w-3 h-2 ml-1" />
      </div>
    </div>

    <!-- Mobile/Tablet Menu Button - Show on LG and below -->
    <button
      class="lg:hidden flex items-center justify-center w-10 h-10 rounded-md border border-white/5 hover:bg-white/5 transition-colors relative z-[60]"
      on:click={toggleMobileMenu}
      aria-label="Toggle menu"
    >
      {#if !isMobileMenuOpen}
        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
        </svg>
      {:else}
        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
        </svg>
      {/if}
    </button>
  </div>
</nav>

<!-- Mobile Menu - Show on LG and below -->
{#if isMobileMenuOpen}
  <!-- Backdrop -->
  <!-- svelte-ignore a11y_click_events_have_key_events -->
  <!-- svelte-ignore a11y_no_static_element_interactions -->
  <div 
    class="lg:hidden fixed inset-0 z-40 bg-black/60 backdrop-blur-sm"
    on:click={closeMobileMenu}
    transition:fade={{ duration: 250 }}
  ></div>
  
  <!-- Mobile Menu Panel -->
  <div 
    class="lg:hidden fixed top-[80px] left-4 right-4 sm:left-6 sm:right-6 md:left-8 md:right-8 z-50 max-h-[calc(100vh-100px)] overflow-y-auto"
    transition:slide={{ duration: 300 }}
  >
    <div class="bg-[rgba(8,6,10,0.95)] backdrop-blur-xl border border-white/10 rounded-2xl shadow-2xl p-4 sm:p-6">
      
      <!-- Close Button (Additional) -->
      <div class="flex justify-end mb-4 lg:hidden">
        <button
          on:click={closeMobileMenu}
          class="flex items-center justify-center w-8 h-8 rounded-full border border-white/20 hover:bg-white/10 transition-colors"
          aria-label="Close menu"
        >
          <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
          </svg>
        </button>
      </div>

      <!-- Navigation Section -->
      <div class="mb-6">
        <h3 class="text-white font-semibold text-lg mb-4 pb-2 border-b border-white/20">Navigation</h3>
        <div class="space-y-1">
          <a href="/get-started" on:click={closeMobileMenu} class="block">
            <div class="w-full text-left px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200 border-b border-white/5">
              <span class="text-[16px] font-medium">Get started</span>
            </div>
          </a>
          <a href="/shop" on:click={closeMobileMenu} class="block">
            <div class="w-full text-left px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200 border-b border-white/5">
              <span class="text-[16px] font-medium">Shop</span>
            </div>
          </a>
          <a href="/about" on:click={closeMobileMenu} class="block">
            <div class="w-full text-left px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200 border-b border-white/5">
              <span class="text-[16px] font-medium">About us</span>
            </div>
          </a>
          <a href="/news" on:click={closeMobileMenu} class="block">
            <div class="w-full text-left px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200 border-b border-white/5">
              <span class="text-[16px] font-medium">News</span>
            </div>
          </a>
          <a href="/contacts" on:click={closeMobileMenu} class="block">
            <div class="w-full text-left px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200 border-b border-white/5">
              <span class="text-[16px] font-medium">Contacts</span>
            </div>
          </a>
          <a href="/faqs" on:click={closeMobileMenu} class="block">
            <div class="w-full text-left px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200">
              <span class="text-[16px] font-medium">FAQs</span>
            </div>
          </a>
        </div>
      </div>

      <!-- Actions Section -->
      <div class="mb-4">
        <h3 class="text-white font-semibold text-lg mb-4 pb-2 border-b border-white/20">Actions</h3>
        <div class="space-y-1">
          <a href="/live" on:click={closeMobileMenu} class="block">
            <div class="w-full flex items-center px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200 border-b border-white/5">
              <img src={Alert} alt="Live" class="w-5 h-5 mr-4" />
              <span class="text-[16px] font-medium">Live</span>
            </div>
          </a>
          <a href="/subscription" on:click={closeMobileMenu} class="block">
            <div class="w-full flex items-center px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200 border-b border-white/5">
              <img src={Star} alt="Subscription" class="w-5 h-5 mr-4" />
              <span class="text-[16px] font-medium">Subscription</span>
            </div>
          </a>
          <a href="/servers" on:click={closeMobileMenu} class="block">
            <div class="w-full flex items-center px-4 py-4 text-white hover:bg-white/15 rounded-lg transition-all duration-200 border-b border-white/5 bg-[#252327]">
              <img src={Data} alt="Servers" class="w-5 h-5 mr-4" />
              <span class="text-[16px] font-medium">Servers</span>
            </div>
          </a>
          <a href="/download" on:click={closeMobileMenu} class="block">
            <div class="w-full flex items-center px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200 border-b border-white/5">
              <img src={File} alt="Download" class="w-5 h-5 mr-4" />
              <span class="text-[16px] font-medium">Download launcher</span>
            </div>
          </a>
          <a href="/notifications" on:click={closeMobileMenu} class="block">
            <div class="w-full flex items-center px-4 py-4 text-white hover:bg-white/10 rounded-lg transition-all duration-200">
              <img src={Bell} alt="Notifications" class="w-5 h-5 mr-4" />
              <span class="text-[16px] font-medium">Notifications</span>
            </div>
          </a>
        </div>
      </div>

      <!-- User Profile Section -->
      <div class="pt-4 border-t border-white/20">
        <div class="flex items-center px-4 py-3 bg-purple-800 rounded-lg">
          <img src={Avatar} alt="User Avatar" class="w-8 h-8 rounded-full border border-white/5 mr-4" />
          <div class="flex-1">
            <span class="text-white font-medium text-[16px]">JohnDoe_911</span>
            <p class="text-white/70 text-sm">View Profile</p>
          </div>
          <img src={Arrow} alt="Arrow" class="w-3 h-2" />
        </div>
      </div>
    </div>
  </div>
{/if}





<style>
  /* Smooth transitions */
  button {
    transition: background-color 0.3s ease;
  }
  
  /* Ensure proper text color */
  button, a {
    color: white;
  }

  /* Mobile menu styling */
  .space-y-1 > :not([hidden]) ~ :not([hidden]) {
    margin-top: 0.25rem;
  }

  /* Custom scrollbar */
  .overflow-y-auto::-webkit-scrollbar {
    width: 6px;
  }
  
  .overflow-y-auto::-webkit-scrollbar-track {
    background: rgba(255, 255, 255, 0.1);
    border-radius: 3px;
  }
  
  .overflow-y-auto::-webkit-scrollbar-thumb {
    background: rgba(255, 255, 255, 0.3);
    border-radius: 3px;
  }
  
  .overflow-y-auto::-webkit-scrollbar-thumb:hover {
    background: rgba(255, 255, 255, 0.5);
  }

  /* Ensure mobile menu button is always visible */
  .z-\[60\] {
    z-index: 60;
  }
</style>