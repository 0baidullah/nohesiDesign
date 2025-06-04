<!-- src/routes/+layout.svelte -->
<script>
  import '../app.css'; // if you have global styles
  import Header from '../lib/+Header.svelte';
  import Footer from '../lib/+Footer.svelte';
</script>

<div class="antialiased bg-black text-white">
  <Header />
  <main class="flex flex-col items-center justify-center min-h-screen ">
    <slot />
  </main>
  <Footer />
</div>