<script lang="ts">
	import '../app.css';
	import { Navigation } from '$lib';

	let { children } = $props();
</script>

<svelte:head>
  <link href="https://fonts.googleapis.com/css2?family=Lustria&family=Open+Sans:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    html { font-family: 'Open Sans', Arial, sans-serif; }
    h1, h2, h3, h4, h5, h6 { font-family: 'Lustria', serif; }
  </style>
</svelte:head>

<div class="relative min-h-screen w-full">
  <div class="absolute left-0 right-0 z-50 pt-8">
    <div class="sticky top-0 flex justify-center w-full">
      <Navigation />
    </div>
  </div>
  {@render children()}
  <footer class="w-full py-6 flex justify-center items-center">
    <a href="/impressum" class="text-[#768680] underline hover:text-[#5e6b63] transition">Impressum</a>
  </footer>
</div>
