<!-- <script>
  const features = [
    "Access to 100+ public servers",
    "Monthly public car updates",
    "Help & FAQ support",
  ];
  import Tier from "../lib/assets/tier0.png";
  import Tick from "../lib/assets/fi_1008958.png";
</script>

<div class="w-[1368px] h-[639px] rounded-2xl border border-white/5">
  <div
    class="w-[342px] h-[639px] gap-2 bg-black text-white p-4 rounded-2xl border border-white/5 flex flex-col shadow-md"
  >
    <div class="w-[294px] h-[20px] flex items-center gap-2">
      <img src={Tier} alt="Tier 0" class="w-4 h-4 object-cover rounded-lg" />
      <div
        class="font-['Roboto_Flex'] font-bold italic text-[16px] leading-5 tracking-normal uppercase"
      >
        TIER 0
      </div>
    </div>
    <div class="w-[294px] h-[85px]">
      <div
        class="font-inter-tight font-semibold text-[20px] leading-[1] tracking-normal"
      >
        Public
      </div>
      <div
        class="font-inter-tight mt-1 font-semibold text-[38px] leading-[48px] tracking-normal"
      >
        Free
      </div>
    </div>
    <div class="w-[294px] h-[76px]">
      <button
        class="w-[294px] h-[52px] rounded-lg px-[77px] py-4 flex items-center gap-5"
        style="background: #252327;"
      >
        <div
          class=" w-[139px] h-[20px] font-['Roboto_Flex'] font-bold italic text-center text-[16px] leading-5 tracking-normal uppercase"
        >
          current plane
        </div>
      </button>

      <button class=" w-[114px] h-[25px] flex items-center mt-2 ml-[90px]">
        <img src={Gift} alt="Gift Icon" class="inline-block w-3.5 h-3.5 mr-1" />

        <div
          class=" w-[192px] h-[25px] items-center justify-center font-['Roboto_Flex'] font-bold italic text-[15px] leading-[25px] underline underline-offset-3"
          style="color: #ACABAD;"
        >
          Send as a Gift
        </div>
      </button>
    </div>

    <ul class=" flex flex-col gap-3 text-sm mt-6">
      {#each features as feature}
        <li
          class="w-[294px] h-[49px] rounded-2xl border border-white/5 pt-3 pr-4 pb-3 flex items-center gap-2"
        >
          <img
            src={Tick}
            alt="Tick Icon"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <span
            class="font-inter-tight font-medium text-[15px] leading-[25px] tracking-normal"
          >
            {feature}
          </span>
        </li>
      {/each}
    </ul>
  </div>
</div> -->

<script>
  const features = [
    "Access to 100+ public servers",
    "Monthly public car updates",
    "Help & FAQ support",
  ];
  import Tier from "../public/static/assets/tier0.png";
  import Tick from "../public/static/assets/fi_1008958.png";
  import Gift from "../public/static/assets/Gift.png";
  import Tier2 from "../public/static/assets/Cube.png";
  import Tier3 from "../public/static/assets/Tier3.png";
  import Tier4 from "../public/static/assets/Tier4.png";
</script>

<div
  class="w-full px-4 z-0 py-6 grid gap-6
         grid-cols-1 sm:grid-cols-1 md:grid-cols-2 xl:grid-cols-4
         justify-items-center"
>
  <div
    class="w-[342px] h-[639px] gap-2 bg-black text-white p-4 rounded-2xl border border-white/5 flex flex-col shadow-md"
  >
    <div class="w-[294px] h-[20px] flex items-center gap-2">
      <img src={Tier} alt="Tier 0" class="w-4 h-4 object-cover rounded-lg" />
      <div
        class="font-['Roboto_Flex'] font-bold italic text-[16px] leading-5 tracking-normal uppercase"
      >
        TIER 0
      </div>
    </div>

    <div class="w-[294px] h-[85px]">
      <div class="font-inter-tight font-semibold text-[20px] leading-[1]">
        Public
      </div>
      <div
        class="font-inter-tight mt-1 font-semibold text-[38px] leading-[48px]"
      >
        Free
      </div>
    </div>

    <div class="w-[294px] h-[76px]">
      <button
        class="w-[294px] h-[52px] rounded-lg px-[77px] py-4 flex items-center gap-5 bg-[#252327]"
      >
        <div
          class="w-[139px] h-[20px] font-['Roboto_Flex'] font-bold italic text-center text-[16px] uppercase"
        >
          current plan
        </div>
      </button>

      <button class="w-[114px] h-[25px] flex items-center mt-2 ml-[90px]">
        <img src={Gift} alt="Gift Icon" class="w-3.5 h-3.5 mr-1" />
        <div
          class="w-[192px] h-[25px] font-['Roboto_Flex'] font-bold italic text-[15px] leading-[25px] underline underline-offset-3 text-[#ACABAD]"
        >
          Send as a Gift
        </div>
      </button>
    </div>

    <ul class="flex flex-col gap-3 text-sm mt-6">
      {#each features as feature}
        <li
          class="w-[294px] h-[49px] rounded-2xl pt-3 pr-4 pb-3 flex items-center gap-2"
        >
          <img
            src={Tick}
            alt="Tick Icon"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <span class="font-inter-tight font-medium text-[15px] leading-[25px]">
            {feature}
          </span>
        </li>
      {/each}
    </ul>
  </div>
  <div
    class="w-[342px] h-[639px] gap-2 text-white p-4 rounded-2xl border border-white/5 flex flex-col shadow-md bg-black/60 backdrop-blur-md"
    style="
    background:
      linear-gradient(0deg, rgba(8,6,10,0.44), rgba(8,6,10,0.44)),
      radial-gradient(160.5% 100% at 50% 0%, rgba(8,6,10,0.05) 25.18%, rgba(231,223,216,0.05) 100%);
  "
  >
    <div class="w-full flex items-center justify-between">
      <div class="flex items-center gap-2">
        <img src={Tier} alt="Tier 1" class="w-4 h-4 object-cover rounded-lg" />
        <div
          class="font-['Roboto_Flex'] font-bold italic text-[16px] leading-5 tracking-normal uppercase"
        >
          TIER 3
        </div>
      </div>

      <div
        class="w-[54px] h-[30px] text-black text-center font-inter-tight font-bold text-[15px] leading-[1] tracking-normal rounded-full"
        style="background: rgba(106, 255, 103, 1);"
      >
        <p class="pt-1.5">-20%</p>
      </div>
    </div>

    <div class="w-[294px] h-[85px]">
      <div class="font-inter-tight font-semibold text-[20px] leading-[1]">
        Public
      </div>
      <div
        class="font-inter-tight mt-1 font-semibold text-[38px] leading-[48px]"
      >
        $2.2/month
      </div>
    </div>

    <div class="w-[294px] h-[76px]">
      <button
        class="w-[294px] h-[52px] rounded-lg px-[77px] py-4 flex items-center gap-5 bg-[#252327]"
      >
        <div
          class="w-[139px] h-[20px] font-['Roboto_Flex'] font-bold italic text-center text-[16px] uppercase"
        >
          current plan
        </div>
      </button>

      <button class="w-[114px] h-[25px] flex items-center mt-2 ml-[90px]">
        <img src={Gift} alt="Gift Icon" class="w-3.5 h-3.5 mr-1" />
        <div
          class="w-[192px] h-[25px] font-['Roboto_Flex'] font-bold italic text-[15px] leading-[25px] underline underline-offset-3 text-[#ACABAD]"
        >
          Send as a Gift
        </div>
      </button>
    </div>

    <ul class="flex flex-col gap-3 text-sm mt-6">
      {#each features as feature}
        <li
          class="w-[294px] h-[49px] rounded-2xl pt-3 pr-4 pb-3 flex items-center gap-2"
        >
          <img
            src={Tick}
            alt="Tick Icon"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <span class="font-inter-tight font-medium text-[15px] leading-[25px]">
            {feature}
          </span>
        </li>
      {/each}
    </ul>
  </div>
  <div
    class="w-[342px] h-[639px] gap-2 text-white p-4 rounded-2xl border border-white/5 flex flex-col shadow-md bg-black/60 backdrop-blur-md"
    style="
    
      background: radial-gradient(160.5% 100% at 50% 0%, rgba(8, 6, 10, 0.05) 25.18%, rgba(255, 129, 38, 0.05) 100%);
background: radial-gradient(160.5% 100% at 50% 0%, rgba(8, 6, 10, 0.05) 25.18%, rgba(255, 129, 38, 0.05) 100%);

  "
  >
    <div class="w-full flex items-center justify-between">
      <div class="flex items-center gap-2">
        <img
          style=""
          src={Tier3}
          alt="Tier 1"
          class="w-4 h-4 object-cover rounded-lg"
        />
        <div
          class="font-['Roboto_Flex'] font-bold italic text-[16px] leading-5 tracking-normal uppercase"
        >
          TIER 3
        </div>
      </div>

      <div
        class="w-[54px] h-[30px] text-black text-center font-inter-tight font-bold text-[15px] leading-[1] tracking-normal rounded-full"
        style="background: rgba(106, 255, 103, 1);"
      >
        <p class="pt-1.5">-20%</p>
      </div>
    </div>

    <div class="w-[294px] h-[85px]">
      <div class="font-inter-tight font-semibold text-[20px] leading-[1]">
        Public
      </div>
      <div
        class="font-inter-tight mt-1 font-semibold text-[38px] leading-[48px]"
      >
        $2.2/month
      </div>
    </div>

    <div class="w-[294px] h-[76px]">
      <button
        class="w-[294px] h-[52px] rounded-lg px-[77px] py-4 flex items-center gap-5 bg-[#252327]"
      >
        <div
          class="w-[139px] h-[20px] font-['Roboto_Flex'] font-bold italic text-center text-[16px] uppercase"
        >
          current plan
        </div>
      </button>

      <button class="w-[114px] h-[25px] flex items-center mt-2 ml-[90px]">
        <img src={Gift} alt="Gift Icon" class="w-3.5 h-3.5 mr-1" />
        <div
          class="w-[192px] h-[25px] font-['Roboto_Flex'] font-bold italic text-[15px] leading-[25px] underline underline-offset-3 text-[#ACABAD]"
        >
          Send as a Gift
        </div>
      </button>
    </div>

    <ul class="flex flex-col gap-3 text-sm mt-6">
      {#each features as feature}
        <li
          class="w-[294px] h-[49px] rounded-2xl pt-3 pr-4 pb-3 flex items-center gap-2"
        >
          <img
            src={Tick}
            alt="Tick Icon"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <span class="font-inter-tight font-medium text-[15px] leading-[25px]">
            {feature}
          </span>
        </li>
      {/each}
    </ul>
  </div>

  <div class="relative">
    <!-- Discount Tag -->
    <div
      class="w-[342px] h-[50px] overflow-hidden absolute -top-3 left-0 right-0 mx-auto px-3 py-1 text-xs font-bold uppercase text-white rounded-t-xl z-0"
      style="background: rgba(221, 3, 85, 1);
"
    >
      MOST POPULAR
    </div>

    <!-- Original Card Code -->
    <div
      class="w-[342px] relative z-10 h-[639px] gap-2 text-white p-4 rounded-2xl border border-white/5 flex flex-col shadow-md bg-black/60 backdrop-blur-md"
      style="
      background: radial-gradient(160.5% 100% at 50% 0%, rgba(8, 6, 10, 0.22) 25.18%, rgba(254, 44, 85, 0.22) 100%);
    "
    >
      <div class="w-full flex items-center justify-between">
        <div class="flex items-center gap-2">
          <img
            style="box-shadow: 0px 0px 20px 0px rgba(221, 3, 85, 0.7);"
            src={Tier4}
            alt="Tier 1"
            class="w-4 h-4 object-cover rounded-lg"
          />
          <div
            class="font-['Roboto_Flex'] font-bold italic text-[16px] leading-5 tracking-normal uppercase"
          >
            TIER 4
          </div>
        </div>

        <div
          class="w-[54px] h-[30px] text-black text-center font-inter-tight font-bold text-[15px] leading-[1] tracking-normal rounded-full"
          style="background: rgba(106, 255, 103, 1);"
        >
          <p class="pt-1.5">-40%</p>
        </div>
      </div>

      <div class="w-[294px] h-[85px]">
        <div class="font-inter-tight font-semibold text-[20px] leading-[1]">
          Public
        </div>
        <div
          class="font-inter-tight mt-1 font-semibold text-[38px] leading-[48px]"
        >
          $2.2/month
        </div>
      </div>

      <div class="w-[294px] h-[76px]">
        <button
          class="w-[294px] h-[52px] rounded-lg px-[77px] py-4 flex items-center gap-5 bg-[#252327]"
        >
          <div
            class="w-[139px] h-[20px] font-['Roboto_Flex'] font-bold italic text-center text-[16px] uppercase"
          >
            current plan
          </div>
        </button>

        <button class="w-[114px] h-[25px] flex items-center mt-2 ml-[90px]">
          <img src={Gift} alt="Gift Icon" class="w-3.5 h-3.5 mr-1" />
          <div
            class="w-[192px] h-[25px] font-['Roboto_Flex'] font-bold italic text-[15px] leading-[25px] underline underline-offset-3 text-[#ACABAD]"
          >
            Send as a Gift
          </div>
        </button>
      </div>

      <ul class="flex flex-col gap-3 text-sm mt-6">
        {#each features as feature}
          <li
            class="w-[294px] h-[49px] rounded-2xl pt-3 pr-4 pb-3 flex items-center gap-2"
          >
            <img
              src={Tick}
              alt="Tick Icon"
              class="w-4 h-4 object-cover rounded-lg"
            />
            <span
              class="font-inter-tight font-medium text-[15px] leading-[25px]"
            >
              {feature}
            </span>
          </li>
        {/each}
      </ul>
    </div>
  </div>
</div>

`
