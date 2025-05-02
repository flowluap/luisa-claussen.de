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
  <title>Luisa Claussen | Social Media Beratung für lokale Unternehmen</title>
  <meta name="description" content="Luisa Claussen bietet individuelle Social Media Beratung, Strategie und Content für lokale Unternehmen. Jetzt kostenloses Erstgespräch buchen!" />
  <link rel="canonical" href="https://luisa-claussen.de/" />
  <meta name="keywords" content="Social Media Beratung, Social Media Strategie, Social Media Trier, Social Media Consultant, Lokale Unternehmen, Luisa Claussen, Social Media Marketing, Beratung, Content, Buchung" />
  <meta property="og:title" content="Luisa Claussen | Social Media Beratung für lokale Unternehmen" />
  <meta property="og:description" content="Individuelle Social Media Beratung, Strategie und Content für lokale Unternehmen. Jetzt kostenloses Erstgespräch buchen!" />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://luisa-claussen.de/" />
  <meta property="og:image" content="https://luisa-claussen.de/og-image.jpg" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Luisa Claussen | Social Media Beratung für lokale Unternehmen" />
  <meta name="twitter:description" content="Individuelle Social Media Beratung, Strategie und Content für lokale Unternehmen. Jetzt kostenloses Erstgespräch buchen!" />
  <meta name="twitter:image" content="https://luisa-claussen.de/og-image.jpg" />
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
