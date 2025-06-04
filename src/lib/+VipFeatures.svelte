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
  import Tier from "assets/tier0.png";
  import Gift from "assets/Gift.png";
  import Tick from "assets/fi_1008958.png";
</script>

<!-- ✅ Responsive grid wrapper -->
<div
  class="w-full px-4 py-6 grid gap-6
         grid-cols-1 sm:grid-cols-1 md:grid-cols-2 xl:grid-cols-4
         justify-items-center"
>
  <!-- ✅ Card starts -->
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
      <div class="font-inter-tight mt-1 font-semibold text-[38px] leading-[48px]">
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
          class="w-[294px] h-[49px] rounded-2xl border border-white/5 pt-3 pr-4 pb-3 flex items-center gap-2"
        >
          <img src={Tick} alt="Tick Icon" class="w-4 h-4 object-cover rounded-lg" />
          <span
            class="font-inter-tight font-medium text-[15px] leading-[25px]"
          >
            {feature}
          </span>
        </li>
      {/each}
    </ul>
  </div>
  <!-- ✅ Card ends -->

  <!-- 🔁 Duplicate the above card as needed for multiple tiers -->
</div>
