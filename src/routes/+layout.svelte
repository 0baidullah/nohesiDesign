<!-- src/routes/+layout.svelte -->
<script>
// @ts-nocheck

  import '../app.css'; // if you have global styles
  import Header from '../lib/+Header.svelte';
  import Footer from '../lib/+Footer.svelte';
  import Nav from '$lib/+newfot.svelte';
  import NewNav from '../lib/+NewNav.svelte';  
  
</script>

<div class="antialiased  " style="background-color : #08060A;">
  <!-- <Header /> -->
  <NewNav />
  <!-- <Nav /> -->
  <!-- <main class="flex flex-col items-center justify-center min-h-screen " >
    <slot />
  </main> -->
  <!-- <Footer /> -->
</div>