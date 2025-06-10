<script>
  // Import your assets
  import Tier from "$lib/assets/tier0.png";
  import Gift from "$lib/assets/Gift.png";
  import Tick from "$lib/assets/fi_1008958.png";

  // Sample features data
  const features = [
    "Access to basic features",
    "Community support",
    "Standard templates",
    "Basic analytics",
    "Email support",
    "Mobile app access",
    "Cloud storage (1GB)",
    "Basic integrations",
  ];

  // You can make this dynamic by passing props or creating multiple card components
  //   const cardData = {
  //     tier: "TIER 0",
  //     title: "Public",
  //     price: "Free",
  //     isCurrentPlan: true,
  //     features: features,
  //   };

  // make 3 caeds
  const cardData = {
    tier: "TIER 0",
    title: "Public",
    price: "Free",
    isCurrentPlan: true,
    features: features,
  };
</script>

<!-- Responsive Grid Container -->
<div class="w-full px-2 sm:px-4 z-0 py-4 sm:py-6">
  <div
    class="grid gap-4 sm:gap-6
              grid-cols-1
              sm:grid-cols-2
              lg:grid-cols-3
              xl:grid-cols-4
              2xl:grid-cols-4
              justify-items-center max-w-7xl mx-auto"
  >
    <!-- Pricing Card -->
    <div
      class="w-full max-w-sm
                h-auto min-h-[580px] sm:min-h-[620px] lg:min-h-[639px]
                bg-black text-white
                p-4 sm:p-6
                rounded-2xl

                flex flex-col
                transition-all duration-300
            "
    >
      <!-- Tier Header -->
      <div class="w-full flex items-center gap-2 mb-4">
        <img
          src={Tier}
          alt="Tier 0"
          class="w-4 h-4 object-cover rounded-lg flex-shrink-0"
        />
        <div
          class="font-['Roboto_Flex'] font-bold italic
                    text-sm sm:text-base
                    leading-5 tracking-normal uppercase"
        >
          {cardData.tier}
        </div>
      </div>

      <!-- Title and Price -->
      <div class="w-full mb-6 sm:mb-8">
        <div
          class="font-inter-tight font-semibold
                    text-lg sm:text-xl
                    leading-tight mb-1"
        >
          {cardData.title}
        </div>
        <div
          class="font-inter-tight font-semibold
                    text-3xl sm:text-4xl lg:text-[38px]
                    leading-tight sm:leading-[48px]"
        >
          {cardData.price}
        </div>
      </div>

      <!-- Action Buttons -->
      <div class="w-full mb-6 sm:mb-8 flex flex-col items-center gap-3">
        <!-- Primary Button -->
        <button
          class="w-full max-w-[240px]
                       h-11 sm:h-12 lg:h-[52px]
                       rounded-lg
                       px-4 sm:px-6
                       py-2 sm:py-3
                       flex items-center justify-center
                       transition-colors duration-200
                       focus:outline-none focus:ring-2 focus:ring-white/20"
        >
          <div
            class="font-['Roboto_Flex'] font-bold italic
                      text-sm sm:text-base
                      uppercase text-center"
          >
            {cardData.isCurrentPlan ? "Current Plan" : "Select Plan"}
          </div>
        </button>

        <!-- Gift Button -->
        <button
          class="flex items-center gap-1
                       h-6 sm:h-[25px]
                       transition-opacity duration-200
                       focus:outline-none focus:ring-2 focus:ring-white/20 rounded"
        >
          <img
            src={Gift}
            alt="Gift Icon"
            class="w-3 h-3 sm:w-3.5 sm:h-3.5 flex-shrink-0"
          />
          <div
            class="font-['Roboto_Flex'] font-bold italic
                      text-xs sm:text-[13px] lg:text-[15px]
                      leading-[25px]
                      underline underline-offset-2 sm:underline-offset-3
                      text-[#ACABAD]"
          >
            Send as a Gift
          </div>
        </button>
      </div>

      <!-- Features List -->
      <div class="flex-1">
        <ul class="flex flex-col gap-2 sm:gap-3 text-sm">
          {#each cardData.features as feature, index}
            <li
              class="w-full
                       min-h-[40px] sm:min-h-[49px]
                       rounded-xl sm:rounded-2xl
                       p-2 sm:p-3
                       flex items-center gap-2 sm:gap-3
                       transition-colors duration-200"
            >
              <img
                src={Tick}
                alt="Tick Icon"
                class="w-3.5 h-3.5 sm:w-4 sm:h-4
                          object-cover rounded-lg flex-shrink-0"
              />
              <span
                class="font-inter-tight font-medium
                           text-sm sm:text-[15px]
                           leading-5 sm:leading-[25px]
                           text-white/90"
              >
                {feature}
              </span>
            </li>
          {/each}
        </ul>
      </div>
    </div>

    <!-- You can duplicate this card structure for other tiers -->
    <!-- Example: Additional cards with different data -->
    <div
      class="w-full max-w-sm
                h-auto min-h-[580px] sm:min-h-[620px] lg:min-h-[639px]
                bg-gradient-to-br from-black-900/20 to-black-900/20
                text-white
                p-4 sm:p-6
                rounded-2xl
                border border-gray-500/20
                flex flex-col
                transition-all duration-300
                relative overflow-hidden"
      style="background: linear-gradient(0deg, rgba(8, 6, 10, 0.44), rgba(8, 6, 10, 0.44)),
radial-gradient(160.5% 100% at 50% 0%, rgba(8, 6, 10, 0.05) 25.18%, rgba(231, 223, 216, 0.05) 100%);
backdrop-filter: blur(200px)

"
    >
      <!-- Popular Badge -->

      <!-- Tier Header -->
      <div class="w-full flex items-center gap-2 mb-4">
        <img
          src={Tier}
          alt="Tier 0"
          class="w-4 h-4 object-cover rounded-lg flex-shrink-0"
        />
        <div
          class="font-['Roboto_Flex'] font-bold italic
                    text-sm sm:text-base
                    leading-5 tracking-normal uppercase"
        >
          TIER 1
        </div>
      </div>

      <!-- Title and Price -->
      <div class="w-full mb-6 sm:mb-8">
        <div
          class="font-inter-tight font-semibold
                    text-lg sm:text-xl
                    leading-tight mb-1"
        >
          Professional
        </div>
        <div
          class="font-inter-tight font-semibold
                    text-3xl sm:text-4xl lg:text-[38px]
                    leading-tight sm:leading-[48px]"
        >
          $29<span class="text-lg text-white/70">/mo</span>
        </div>
      </div>

      <!-- Action Buttons -->
      <div class="w-full mb-6 sm:mb-8 flex flex-col items-center gap-3">
        <button
          class="w-full max-w-[240px]
                       h-11 sm:h-12 lg:h-[52px]
                       rounded-lg
                       px-4 sm:px-6
                       py-2 sm:py-3
                       flex items-center justify-center
                       transition-all duration-200
                       focus:outline-none focus:ring-2 focus:ring-black-500/50
                       bg-white
                        text-black"
        >
          <div
            class="font-['Roboto_Flex'] font-bold italic
                      text-sm sm:text-base
                      uppercase text-center"
          >
            Upgrade Now
          </div>
        </button>

        <button
          class="flex items-center gap-1
                       h-6 sm:h-[25px]
                       transition-opacity duration-200"
        >
          <img
            src={Gift}
            alt="Gift Icon"
            class="w-3 h-3 sm:w-3.5 sm:h-3.5 flex-shrink-0"
          />
          <div
            class="font-['Roboto_Flex'] font-bold italic
                      text-xs sm:text-[13px] lg:text-[15px]
                      leading-[25px]
                      underline underline-offset-2 sm:underline-offset-3
                      text-gray-300"
          >
            Send as a Gift
          </div>
        </button>
      </div>

      <!-- Features List -->
      <div class="flex-1">
        <ul class="flex flex-col gap-2 sm:gap-3 text-sm">
          {#each ["Everything in Free", "Advanced analytics", "Priority support", "Custom templates", "API access", "10GB storage", "Team collaboration"] as feature}
            <li
              class="w-full
                       min-h-[40px] sm:min-h-[49px]
                       rounded-xl sm:rounded-2xl
                       p-2 sm:p-3
                       flex items-center gap-2 sm:gap-3
                       transition-colors duration-200"
            >
              <div>
                <img
                  src={Tick}
                  alt="Tier 0"
                  class="w-4 h-4 object-cover rounded-lg flex-shrink-0"
                />
              </div>
              <span
                class="font-inter-tight font-medium
                           text-sm sm:text-[15px]
                           leading-5 sm:leading-[25px]
                           text-white/90"
              >
                {feature}
              </span>
            </li>
          {/each}
        </ul>
      </div>
    </div>
    <div
      class="w-full max-w-sm
                h-auto min-h-[580px] sm:min-h-[620px] lg:min-h-[639px]
                text-white
                p-4 sm:p-6
                rounded-2xl
                border border-gray-500/20
                flex flex-col
                transition-all duration-300
                relative overflow-hidden"
      style="background: radial-gradient(160.5% 100% at 50% 0%, rgba(8, 6, 10, 0.05) 25.18%, rgba(255, 129, 38, 0.05) 100%);

backdrop-filter: blur(200px)

"
    >
      <!-- Popular Badge -->

      <!-- Tier Header -->
      <div class="w-full flex items-center gap-2 mb-4">
        <img
          src={Tier}
          alt="Tier 0"
          class="w-4 h-4 object-cover rounded-lg flex-shrink-0"
        />
        <div
          class="font-['Roboto_Flex'] font-bold italic
                    text-sm sm:text-base
                    leading-5 tracking-normal uppercase"
        >
          TIER 1
        </div>
      </div>

      <!-- Title and Price -->
      <div class="w-full mb-6 sm:mb-8">
        <div
          class="font-inter-tight font-semibold
                    text-lg sm:text-xl
                    leading-tight mb-1"
        >
          Professional
        </div>
        <div
          class="font-inter-tight font-semibold
                    text-3xl sm:text-4xl lg:text-[38px]
                    leading-tight sm:leading-[48px]"
        >
          $29<span class="text-lg text-white/70">/mo</span>
        </div>
      </div>

      <!-- Action Buttons -->
      <div class="w-full mb-6 sm:mb-8 flex flex-col items-center gap-3">
        <button
          class="w-full max-w-[240px]
                       h-11 sm:h-12 lg:h-[52px]
                       rounded-lg
                       px-4 sm:px-6
                       py-2 sm:py-3
                       flex items-center justify-center
                       transition-all duration-200
                       focus:outline-none focus:ring-2 focus:ring-black-500/50
                       bg-white
                        text-black"
        >
          <div
            class="font-['Roboto_Flex'] font-bold italic
                      text-sm sm:text-base
                      uppercase text-center"
          >
            Upgrade Now
          </div>
        </button>

        <button
          class="flex items-center gap-1
                       h-6 sm:h-[25px]
                       transition-opacity duration-200"
        >
          <img
            src={Gift}
            alt="Gift Icon"
            class="w-3 h-3 sm:w-3.5 sm:h-3.5 flex-shrink-0"
          />
          <div
            class="font-['Roboto_Flex'] font-bold italic
                      text-xs sm:text-[13px] lg:text-[15px]
                      leading-[25px]
                      underline underline-offset-2 sm:underline-offset-3
                      text-gray-300"
          >
            Send as a Gift
          </div>
        </button>
      </div>

      <!-- Features List -->
      <div class="flex-1">
        <ul class="flex flex-col gap-2 sm:gap-3 text-sm">
          {#each ["Everything in Free", "Advanced analytics", "Priority support", "Custom templates", "API access", "10GB storage", "Team collaboration"] as feature}
            <li
              class="w-full
                       min-h-[40px] sm:min-h-[49px]
                       rounded-xl sm:rounded-2xl
                       p-2 sm:p-3
                       flex items-center gap-2 sm:gap-3
                       transition-colors duration-200"
            >
              <div>
                <img
                  src={Tick}
                  alt="Tier 0"
                  class="w-4 h-4 object-cover rounded-lg flex-shrink-0"
                />
              </div>
              <span
                class="font-inter-tight font-medium
                           text-sm sm:text-[15px]
                           leading-5 sm:leading-[25px]
                           text-white/90"
              >
                {feature}
              </span>
            </li>
          {/each}
        </ul>
      </div>
    </div>

    <div
      class="w-full max-w-sm
                h-auto min-h-[580px] sm:min-h-[620px] lg:min-h-[639px]
                text-white
                p-4 sm:p-6
                rounded-2xl
                border border-gray-500/20
                flex flex-col
                relative overflow-hidden"
      style="background: radial-gradient(160.5% 100% at 50% 0%, rgba(8, 6, 10, 0.22) 25.18%, rgba(254, 44, 85, 0.22) 100%);
backdrop-filter: blur(200px)"
    >
      <!-- Popular Badge -->
      <div
        class="absolute -top-1 -right-0
                 
        w-full
                  text-white text-xs font-bold
                   py-1 rounded-bl-lg rounded-tr-2xl
                  "
        style="background: #DD0355;
"
      >
        <p class="px-3.5">Popular</p>
      </div>

      <!-- Tier Header -->
      <div class="w-full flex items-center gap-2 mb-4">
        <img
          src={Tier}
          alt="Tier 0"
          class="w-4 h-4 object-cover rounded-lg flex-shrink-0"
        />
        <div
          class="font-['Roboto_Flex'] font-bold italic
                    text-sm sm:text-base
                    leading-5 tracking-normal uppercase"
        >
          TIER 1
        </div>
      </div>

      <!-- Title and Price -->
      <div class="w-full mb-6 sm:mb-8">
        <div
          class="font-inter-tight font-semibold
                    text-lg sm:text-xl
                    leading-tight mb-1"
        >
          Professional
        </div>
        <div
          class="font-inter-tight font-semibold
                    text-3xl sm:text-4xl lg:text-[38px]
                    leading-tight sm:leading-[48px]"
        >
          $29<span class="text-lg text-white/70">/mo</span>
        </div>
      </div>

      <!-- Action Buttons -->
      <div class="w-full mb-6 sm:mb-8 flex flex-col items-center gap-3">
        <button
          class="w-full max-w-[240px]
                       h-11 sm:h-12 lg:h-[52px]
                       rounded-lg
                       px-4 sm:px-6
                       py-2 sm:py-3
                       flex items-center justify-center
                       transition-all duration-200
                       focus:outline-none focus:ring-2 focus:ring-purple-500/50
                       bg-white
                        text-black"
        >
          <div
            class="font-['Roboto_Flex'] font-bold italic
                      text-sm sm:text-base
                      uppercase text-center"
          >
            Upgrade Now
          </div>
        </button>

        <button
          class="flex items-center gap-1
                       h-6 sm:h-[25px]
                       transition-opacity duration-200"
        >
          <img
            src={Gift}
            alt="Gift Icon"
            class="w-3 h-3 sm:w-3.5 sm:h-3.5 flex-shrink-0"
          />
          <div
            class="font-['Roboto_Flex'] font-bold italic
                      text-xs sm:text-[13px] lg:text-[15px]
                      leading-[25px]
                      underline underline-offset-2 sm:underline-offset-3
                      text-gray-300"
          >
            Send as a Gift
          </div>
        </button>
      </div>

      <!-- Features List -->
      <div class="flex-1">
        <ul class="flex flex-col gap-2 sm:gap-3 text-sm">
          {#each ["Everything in Free", "Advanced analytics", "Priority support", "Custom templates", "API access", "10GB storage", "Team collaboration"] as feature}
            <li
              class="w-full
                       min-h-[40px] sm:min-h-[49px]
                       rounded-xl sm:rounded-2xl
                       p-2 sm:p-3
                       flex items-center gap-2 sm:gap-3


                       transition-colors duration-200"
            >
              <div class="">
                <img
                  src={Tick}
                  alt="Tier 0"
                  class="w-4 h-4 object-cover rounded-lg flex-shrink-0"
                />
              </div>
              <span
                class="font-inter-tight font-medium
                           text-sm sm:text-[15px]
                           leading-5 sm:leading-[25px]
                           text-white/90"
              >
                {feature}
              </span>
            </li>
          {/each}
        </ul>
      </div>
    </div>
  </div>
</div>

<!-- <style>
  /* Ensure fonts load properly */
  :global(@import url('https://fonts.googleapis.com/css2?family=Roboto+Flex:ital,wght@0,400;0,700;1,400;1,700&family=Inter+Tight:wght@400;500;600&display=swap'));
  
  /* Custom scrollbar if needed */
  :global(body) {
    scrollbar-width: thin;
  }
</style> -->
