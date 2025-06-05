<script>
  import Contact from "../../lib/+Contact.svelte";
  import DarkStrip from "../../lib/+spacing.svelte";
  import Plane from "../../lib/+Choseplane.svelte";
  import Feature from "../../lib/+VipFeatures.svelte";
  import Limits from "$lib/+Limits.svelte";
</script>

<div class="antialiased bg-black text-white">
  <DarkStrip />
  <DarkStrip />
  <Plane />
  <DarkStrip />

  <Feature />
  <DarkStrip/>
  <Limits />

  <DarkStrip />
  <Contact />
  <!-- <DarkStrip /> -->
</div>
