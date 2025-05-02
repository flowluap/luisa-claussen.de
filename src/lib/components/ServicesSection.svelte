<section class="py-20 bg-transparent" id="services-section">
  <h2 class="text-2xl font-bold text-center mb-10 relative" style="color: #e9e5dc;">
    Meine Leistungen
    <span class="block h-1 w-16 mx-auto mt-2 rounded-full bg-gradient-to-r from-[#768680] via-[#a0ada7] to-[#e9e5dc] opacity-60"></span>
  </h2>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-10 max-w-5xl mx-auto px-4">
    <div class="flex flex-col items-center text-center">
      <span class="mb-4">
        <!-- Compass Icon -->
        <svg xmlns="http://www.w3.org/2000/svg" class="w-12 h-12" fill="none" viewBox="0 0 24 24" stroke="#e9e5dc" stroke-width="2">
          <circle cx="12" cy="12" r="10" stroke="#e9e5dc" stroke-width="2" fill="none"/>
          <polygon points="12,7 15,17 12,15 9,17" fill="#e9e5dc" stroke="#e9e5dc" stroke-width="1"/>
        </svg>
      </span>
      <h3 class="font-bold text-lg mb-2 text-[#768680]">Strategie-Entwicklung</h3>
      <p class="text-[#768680]">Individuelle Social Media Strategien, die zu Ihren Unternehmenszielen und Ihrer Zielgruppe passen.</p>
    </div>
    <div class="flex flex-col items-center text-center">
      <span class="mb-4">
        <!-- Chat Bubble Icon -->
        <svg xmlns="http://www.w3.org/2000/svg" class="w-12 h-12" fill="none" viewBox="0 0 24 24" stroke="#e9e5dc" stroke-width="2">
          <path d="M21 11.5a8.38 8.38 0 0 1-1.9 5.4c-.5.6-.7 1.4-.5 2.2.2.7-.5 1.3-1.2 1.1-2.2-.7-4.2-1.7-6.1-3.1-2.2-1.6-4-3.7-5.2-6.1-.3-.6.1-1.4.8-1.5.8-.2 1.6-.4 2.3-.7.7-.3 1.1-1.1.9-1.8-.3-1.1-.5-2.2-.5-3.3 0-.7.6-1.3 1.3-1.3h.2c4.7 0 8.5 3.8 8.5 8.5z" stroke="#e9e5dc" stroke-width="2" fill="none"/>
        </svg>
      </span>
      <h3 class="font-bold text-lg mb-2 text-[#768680]">Beratung & Betreuung</h3>
      <p class="text-[#768680]">Persönliche Beratung und laufende Unterstützung für Ihren Social Media Auftritt – unkompliziert & praxisnah.</p>
    </div>
    <div class="flex flex-col items-center text-center">
      <span class="mb-4">
        <!-- Lightbulb Icon -->
        <svg xmlns="http://www.w3.org/2000/svg" class="w-12 h-12" fill="none" viewBox="0 0 24 24" stroke="#e9e5dc" stroke-width="2">
          <path d="M12 2a7 7 0 0 1 7 7c0 2.5-1.5 4.5-3.5 5.5V17a1.5 1.5 0 0 1-3 0v-2.5C6.5 13.5 5 11.5 5 9a7 7 0 0 1 7-7z" stroke="#e9e5dc" stroke-width="2" fill="none"/>
          <rect x="10" y="19" width="4" height="2" rx="1" fill="#e9e5dc"/>
        </svg>
      </span>
      <h3 class="font-bold text-lg mb-2 text-[#768680]">Content-Ideen & Umsetzung</h3>
      <p class="text-[#768680]">Kreative Content-Ideen und praktische Tipps zur Umsetzung, damit Ihre Kanäle lebendig bleiben.</p>
    </div>
  </div>
  <div class="flex justify-center mt-12">
    <button on:click={() => document.getElementById('calendly-section')?.scrollIntoView({ behavior: 'smooth' })}
      class="bg-[#768680] hover:bg-[#5e6b63] text-white font-bold py-3 px-8 rounded-full shadow-lg transition-all">
      Jetzt Termin sichern
    </button>
  </div>
</section> 