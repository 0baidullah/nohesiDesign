<!-- src/routes/+layout.svelte -->
<script>
  import '../app.css'; // if you have global styles
  import Header from '../lib/+Header.svelte';
  import Footer from '../lib/+Footer.svelte';
  import NewNav from '$lib/+NewNav.svelte';
</script>

<div class="antialiased  " style="background-color : #08060A;">
  <!-- <Header /> -->
  <NewNav />
  <!-- <main class="flex flex-col items-center justify-center min-h-screen " >
    <slot />
  </main> -->
  <!-- <Footer /> -->
</div>