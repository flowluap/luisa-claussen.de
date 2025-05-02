<section id="about-section" class="flex flex-col md:flex-row items-center gap-10 py-20 max-w-5xl mx-auto px-4 mt-12">
  <!-- Add to your <head>: <link href='https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap' rel='stylesheet'> -->
  <div class="flex-1 flex flex-col items-start justify-center">
    <span class="inline-flex items-center mb-3 px-4 py-1 bg-[#e9e5dc] text-[#768680] rounded-full font-semibold text-sm shadow-sm">
      <svg class="w-5 h-5 mr-2 text-[#a0ada7]" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13 16h-1v-4h-1m1-4h.01M12 20.5C6.753 20.5 2 15.747 2 10.5S6.753.5 12 .5s10 4.753 10 10-4.753 10-10 10z"/></svg>
      Über Luisa
    </span>
    <h2 class="text-2xl font-bold mb-2 relative" style="color: #e9e5dc;">
      Ihre Social Media Partnerin
      <span class="block h-1 w-16 mt-1 rounded-full bg-gradient-to-r from-[#768680] via-[#a0ada7] to-[#e9e5dc] opacity-60"></span>
    </h2>
    <p class="text-[#768680] mb-2 text-lg">Hi, ich bin Luisa Claussen – Social Media Enthusiastin mit einem Bachelor in Medien & Kommunikation. Ich liebe es, lokale Unternehmen dabei zu unterstützen, online sichtbar und erfolgreich zu werden!</p>
    <blockquote class="italic text-[#768680] bg-[#e9e5dc] rounded-xl px-4 py-2 my-4 border-l-4 border-[#a0ada7] shadow-sm">"Social Media ist mehr als nur Posts – es ist die Chance, echte Beziehungen zu Ihrer Zielgruppe aufzubauen."</blockquote>
    <ul class="list-disc pl-5 text-[#768680] mb-4">
      <li>Erfahrung in der Medien- & Kommunikationsbranche</li>
      <li>Individuelle Beratung, die Spaß macht</li>
      <li>Immer am Puls der Social Trends</li>
    </ul>
    <button on:click={() => document.getElementById('calendly-section')?.scrollIntoView({ behavior: 'smooth' })}
      class="bg-[#768680] hover:bg-[#5e6b63] text-white font-bold py-2 px-6 rounded-full shadow-md transition-all mt-2">
      Jetzt Termin sichern
    </button>
  </div>
  <div class="flex-1 flex justify-center items-center">
    <div class="relative">
      <img src="/src/lib/assets/DSC07347.JPG" alt="Luisa Claussen Portrait" class="w-64 h-64 md:w-80 md:h-80 rounded-2xl object-cover shadow-2xl ring-4 ring-[#e9e5dc]" />
      <span class="absolute -top-4 -right-4 bg-[#a0ada7] text-white px-3 py-1 rounded-full text-xs font-bold shadow-lg rotate-6">#SocialPassion</span>
    </div>
  </div>
</section> 