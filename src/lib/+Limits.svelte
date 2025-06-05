<script>
  const tiers = [
    {
      name: "TIER 0",
      color: "text-gray-400",
      bgColor: "bg-gray-500",
      button: "CURRENT PLAN",
      buttonClass: "bg-gray-600 text-gray-300 cursor-not-allowed",
      isActive: false,
    },
    {
      name: "TIER 1",
      color: "text-white",
      bgColor: "bg-white",
      button: "SUBSCRIBE",
      buttonClass: "bg-white text-black hover:bg-gray-100",
      isActive: false,
    },
    {
      name: "TIER 2",
      color: "text-orange-500",
      bgColor: "bg-orange-500",
      button: "FREE 7-DAYS TRIAL",
      buttonClass: "bg-orange-500 text-white hover:bg-orange-600",
      isActive: false,
    },
    {
      name: "TIER 3",
      color: "text-red-500",
      bgColor: "bg-red-500",
      button: "SUBSCRIBE",
      buttonClass: "bg-red-500 text-white hover:bg-red-600",
      isActive: false,
    },
  ];

  import Tier0 from "../public/static/assets/tier0.png";
  import Tier2 from "../public/static/assets/Cube.png";
  import Tier3 from "../public/static/assets/Tier3.png";
  import Tier4 from "../public/static/assets/Tier4.png";
</script>

<div class="w-full h-[101px] px-9">
  <div class="flex justify-end">
    <div class="grid grid-cols-4 rounded-2xl border border-white/5">
      <div class="w-[300px] h-[101px]">
        <div
          class="w-[280px] h-[20px] justify-center py-4 flex text-center items-center gap-2"
        >
          <img
            src={Tier0}
            alt="Tier 0"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <div
            class="font-['Roboto_Flex'] justify-center font-bold italic text-[16px] leading-5 tracking-normal uppercase"
          >
            TIER 0
          </div>
        </div>
        <button
          class="w-[220px] h-[36px] ml-8 justify-center rounded-lg px-4 flex items-center gap-5 bg-white"
        >
          <div
            class=" font-['Roboto_Flex'] justify-center text-black font-bold italic text-center text-[16px] uppercase"
          >
            currentas plan
          </div>
        </button>
      </div>

      <div class="w-[280px] h-[101px]">
        <div
          class="w-[280px] h-[20px] justify-center py-4 flex text-center items-center gap-2"
        >
          <img
            src={Tier0}
            alt="Tier 0"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <div
            class="font-['Roboto_Flex'] justify-center font-bold italic text-[16px] leading-5 tracking-normal uppercase"
          >
            TIER 1
          </div>
        </div>
        <button
          class="w-[220px] h-[36px] ml-8 justify-center rounded-lg px-4 flex items-center gap-5 bg-white"
        >
          <div
            class=" font-['Roboto_Flex'] text-black justify-center font-bold italic text-center text-[16px] uppercase"
          >
            currentas plan
          </div>
        </button>
      </div>
      <div class="w-[280px] h-[101px]">
        <div
          class="w-[280px] h-[20px] justify-center py-4 flex text-center items-center gap-2"
        >
          <img
            src={Tier3}
            alt="Tier 0"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <div
            class="font-['Roboto_Flex'] justify-center font-bold italic text-[16px] leading-5 tracking-normal uppercase"
          >
            TIER 2
          </div>
        </div>
        <button
          class="w-[220px] h-[36px] text-black ml-8 justify-center rounded-lg px-4 flex items-center gap-5 bg-white"
        >
          <div
            class=" font-['Roboto_Flex'] justify-center font-bold italic text-center text-[16px] uppercase"
          >
            currentas plan
          </div>
        </button>
      </div>
      <div class="w-[280px] h-[101px]">
        <div
          class="w-[280px] h-[20px] justify-center py-4 flex text-center items-center gap-2"
        >
          <img
            src={Tier4}
            alt="Tier 0"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <div
            class="font-['Roboto_Flex'] justify-center font-bold italic text-[16px] leading-5 tracking-normal uppercase"
          >
            TIER 3
          </div>
        </div>
        <button
          class="w-[220px] h-[36px] text-black ml-8 justify-center rounded-lg px-4 flex items-center gap-5 bg-white"
        >
          <div
            class=" font-['Roboto_Flex'] justify-center font-bold italic text-center text-[16px] uppercase"
          >
            currentas plan
          </div>
        </button>
      </div>
    </div>
  </div>
</div>

<div class="w-full h-[48px] px-9">
  <div class="flex justify-end">
    <div class="grid grid-cols-5 rounded-2xl border border-white/5">
      <div class="w-[300px] h-[48px]">
        <div class="w-[280px] h-[20px] justify-start py-4 flex gap-2">
          <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
            Features
          </div>
        </div>
      </div>
      <div class="w-[280px] h-[48px]">
        <div class="w-[280px] h-[20px] justify-center py-4 flex gap-2">
          <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
            Get a chance
          </div>
        </div>
      </div>
      <div class="w-[280px] h-[48px]">
        <div class="w-[280px] h-[20px] justify-center py-4 flex gap-2">
          <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
            Everything You need to know
          </div>
        </div>
      </div>
      <div class="w-[280px] h-[48px]">
        <div class="w-[280px] h-[20px] justify-center py-4 flex gap-2">
          <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
            Amplifi you experience
          </div>
        </div>
      </div>
      <div class="w-[280px] h-[48px]">
        <div class="w-[280px] h-[20px] justify-center py-4 flex gap-2">
          <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
            Reach new limits
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="w-full h-[101px] px-9">
  <div class="flex justify-end">
    <table class="table-fixed border border-white/5 rounded-2xl w-auto">
      <thead>
        <tr class="h-[101px]">
          <!-- TIER 0 -->
          <th class="w-[300px] p-2">
            <div class="flex items-center gap-2 justify-center py-4">
              <img src={Tier0} alt="Tier 0" class="w-4 h-4 object-cover rounded-lg" />
              <div class="font-['Roboto_Flex'] font-bold italic text-[16px] uppercase">
                TIER 0
              </div>
            </div>
            <button class="w-[220px] h-[36px] mx-auto block rounded-lg px-4 bg-white flex items-center justify-center">
              <div class="font-['Roboto_Flex'] text-black font-bold italic text-[16px] uppercase">
                currentas plan
              </div>
            </button>
          </th>
          <th class="w-[300px] p-2">
            <div class="flex items-center gap-2 justify-center py-4">
              <img src={Tier0} alt="Tier 0" class="w-4 h-4 object-cover rounded-lg" />
              <div class="font-['Roboto_Flex'] font-bold italic text-[16px] uppercase">
                TIER 0
              </div>
            </div>
            <button class="w-[220px] h-[36px] mx-auto block rounded-lg px-4 bg-white flex items-center justify-center">
              <div class="font-['Roboto_Flex'] text-black font-bold italic text-[16px] uppercase">
                currentas plan
              </div>
            </button>
          </th>

          <!-- TIER 1 -->
          <th class="w-[300px] p-2">
            <div class="flex items-center gap-2 justify-center py-4">
              <img src={Tier0} alt="Tier 1" class="w-4 h-4 object-cover rounded-lg" />
              <div class="font-['Roboto_Flex'] font-bold italic text-[16px] uppercase">
                TIER 1
              </div>
            </div>
            <button class="w-[220px] h-[36px] mx-auto block rounded-lg px-4 bg-white flex items-center justify-center">
              <div class="font-['Roboto_Flex'] text-black font-bold italic text-[16px] uppercase">
                currentas plan
              </div>
            </button>
          </th>

          <!-- TIER 2 -->
          <th class="w-[300px] p-2">
            <div class="flex items-center gap-2 justify-center py-4">
              <img src={Tier3} alt="Tier 2" class="w-4 h-4 object-cover rounded-lg" />
              <div class="font-['Roboto_Flex'] font-bold italic text-[16px] uppercase">
                TIER 2
              </div>
            </div>
            <button class="w-[220px] h-[36px] mx-auto block rounded-lg px-4 bg-white flex items-center justify-center">
              <div class="font-['Roboto_Flex'] text-black font-bold italic text-[16px] uppercase">
                currentas plan
              </div>
            </button>
          </th>

          <!-- TIER 3 -->
          <th class="w-[300px] p-2">
            <div class="flex items-center gap-2 justify-center py-4">
              <img src={Tier4} alt="Tier 3" class="w-4 h-4 object-cover rounded-lg" />
              <div class="font-['Roboto_Flex'] font-bold italic text-[16px] uppercase">
                TIER 3
              </div>
            </div>
            <button class="w-[220px] h-[36px] mx-auto block rounded-lg px-4 bg-white flex items-center justify-center">
              <div class="font-['Roboto_Flex'] text-black font-bold italic text-[16px] uppercase">
                currentas plan
              </div>
            </button>
          </th>
        </tr>
      </thead>

      <tbody>
        <tr class="h-[48px]">
          <!-- Column 1 -->
          <td class="w-[300px] text-left px-4">
            <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
              Features
            </div>
          </td>

          <!-- Column 2 -->
          <td class="w-[280px] text-center px-4">
            <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
              Get a chance
            </div>
          </td>

          <!-- Column 3 -->
          <td class="w-[280px] text-center px-4">
            <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
              Everytding You need to know
            </div>
          </td>

          <!-- Column 4 -->
          <td class="w-[280px] text-center px-4">
            <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
              Amplifi you experience
            </div>
          </td>

          <!-- Column 5 -->
          <td class="w-[280px] text-center px-4">
            <div class="font-inter-tight text-[18px] leading-5 tracking-normal">
              Reach new limits
            </div>
          </td>
        </tr>
      </tbody>
      
    </table>
  </div>
</div>






<style>
  :global(body) {
    background-color: rgb(17, 24, 39);
    color: white;
    margin: 0;
    padding: 0;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
      sans-serif;
  }
</style>
