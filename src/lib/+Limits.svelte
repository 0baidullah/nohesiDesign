<script>
  const tiers = [
    {
      name: "TIER 0",
      color: "text-gray-400",
      bgColor: "bg-gray-500",
      buttonText: "CURRENT PLAN",
      buttonClass: "bg-gray-600 text-gray-300 cursor-not-allowed",
      isActive: false,
      icon : Tier0,
      description: 'Get a chance'
    },
    {
      name: "TIER 1",
      color: "text-white",
      bgColor: "bg-white",
      buttonText: "SUBSCRIBE",
      buttonClass: "bg-white text-black hover:bg-gray-100",
      isActive: false,
      icon: Tier0,
      description: 'Everything You need to know'
    },
    {
      name: "TIER 2",
      color: "text-orange-500",
      bgColor: "bg-orange-500",
      buttonText: "FREE 7-DAYS TRIAL",
      buttonClass: "bg-orange-500 text-white hover:bg-orange-600",
      isActive: false,
      icon: Tier3,
      description: 'Amplify your experience'
    },
    {
      name: "TIER 3",
      color: "text-red-500",
      bgColor: "bg-red-500",
      buttonText: "SUBSCRIBE",
      buttonClass: "bg-red-500 text-white hover:bg-red-600",
      isActive: false,
      icon: Tier4,
      description: 'Reach new limits'
    },
  ];

  import Tier0 from "../public/static/assets/tier0.png";
  import Tier2 from "../public/static/assets/Cube.png";
  import Tier3 from "../public/static/assets/Tier3.png";
  import Tier4 from "../public/static/assets/Tier4.png";
</script>






<div class="w-full px-4 md:px-9">
  <!-- Desktop/Tablet Table View -->
  <div class="hidden lg:block">
    <div class="overflow-x-auto">
      <table class="min-w-full border border-white/5 rounded-2xl bg-black/20 backdrop-blur-sm">
        <thead>
          <tr class="h-[101px]">
            <!-- Features Column -->
            <th class="w-[300px] p-2 text-left">
              <div class="font-['Inter_Tight'] text-[18px] leading-5 tracking-normal text-white/80 px-4">
                Features
              </div>
            </th>
            
            <!-- Tier Columns -->
            {#each tiers as tier}
              <th class="w-[280px] p-2">
                <div class="flex items-center gap-2 justify-center py-4">
                  <img src={tier.icon} alt={tier.name} class="w-4 h-4 object-cover rounded-lg" />
                  <div class="font-['Roboto_Flex'] font-bold italic text-[16px] uppercase text-white">
                    {tier.name}
                  </div>
                </div>
                <button class="w-[220px] h-[36px] mx-auto block rounded-lg px-4 bg-white hover:bg-gray-100 transition-colors duration-200 flex items-center justify-center">
                  <div class="font-['Roboto_Flex'] text-black font-bold italic text-[16px] uppercase">
                    {tier.buttonText}
                  </div>
                </button>
              </th>
            {/each}
          </tr>
        </thead>

        <tbody>
          <tr class="h-[48px] border-t border-white/5">
            <td class="w-[300px] text-left px-4">
              <div class="font-['Inter_Tight'] text-[18px] leading-5 tracking-normal text-white">
                Features
              </div>
            </td>
            {#each tiers as tier}
              <td class="w-[280px] text-center px-4">
                <div class="font-['Inter_Tight'] text-[16px] leading-5 tracking-normal text-white/80">
                  {tier.description}
                </div>
              </td>
            {/each}
          </tr>
        </tbody>
      </table>
    </div>
  </div>

  <!-- Mobile/Tablet Card View -->
  <div class="lg:hidden">
    <div class="grid grid-cols-1 sm:grid-cols-2 xl:grid-cols-3 gap-4">
      {#each tiers as tier}
        <div class="border border-white/10 rounded-2xl p-6 bg-black/20 backdrop-blur-sm hover:border-white/20 transition-colors duration-200">
          <!-- Tier Header -->
          <div class="flex items-center gap-3 justify-center mb-6">
            <img src={tier.icon} alt={tier.name} class="w-5 h-5 object-cover rounded-lg" />
            <div class="font-['Roboto_Flex'] font-bold italic text-[18px] uppercase text-white">
              {tier.name}
            </div>
          </div>

          <!-- Description -->
          <div class="text-center mb-6">
            <div class="font-['Inter_Tight'] text-[16px] leading-6 tracking-normal text-white/80">
              {tier.description}
            </div>
          </div>

          <!-- Action Button -->
          <button class="w-full h-[44px] rounded-lg px-4 bg-white hover:bg-gray-100 transition-colors duration-200 flex items-center justify-center">
            <div class="font-['Roboto_Flex'] text-black font-bold italic text-[16px] uppercase">
              {tier.buttonText}
            </div>
          </button>
        </div>
      {/each}
    </div>
  </div>

  <!-- Extra Small Mobile - Stacked View -->
  <div class="sm:hidden">
    <div class="space-y-3">
      {#each tiers as tier}
        <div class="border border-white/10 rounded-xl p-4 bg-black/20 backdrop-blur-sm">
          <!-- Compact Tier Header -->
          <div class="flex items-center gap-2 mb-3">
            <img src={tier.icon} alt={tier.name} class="w-4 h-4 object-cover rounded" />
            <div class="font-['Roboto_Flex'] font-bold italic text-[14px] uppercase text-white">
              {tier.name}
            </div>
          </div>

          <!-- Compact Description -->
          <div class="mb-3">
            <div class="font-['Inter_Tight'] text-[14px] leading-5 text-white/80">
              {tier.description}
            </div>
          </div>

          <!-- Compact Button -->
          <button class="w-full h-[36px] rounded-lg px-3 bg-white hover:bg-gray-100 transition-colors duration-200 flex items-center justify-center">
            <div class="font-['Roboto_Flex'] text-black font-bold italic text-[14px] uppercase">
              {tier.buttonText}
            </div>
          </button>
        </div>
      {/each}
    </div>
  </div>
</div>



<style>
 
</style>
