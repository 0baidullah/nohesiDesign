<!-- src/routes/+layout.svelte -->
<script>
// @ts-nocheck

  import '../app.css'; // if you have global styles
  import Header from '../lib/+Header.svelte';
  import Footer from '../lib/+Footer.svelte';
  import Nav from '$lib/+newfot.svelte';
  import NewNav from '../lib/+NewNav.svelte';  
  
</script>

<div class=" "  style=" color: white; max-width: 100%; max-height: 100%;">
  <!-- <Header /> -->
  <NewNav />
  <!-- <Nav /> -->
  <main  class=" max-w-full max-h-full" >
    <slot />
  </main>
  <!-- <Footer /> -->
</div>