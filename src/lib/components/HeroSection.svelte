<section class="flex flex-col md:flex-row items-center md:items-center justify-between bg-gradient-to-br from-[#e9e5dc] via-white to-[#768680] px-4 md:px-16 min-h-[70vh] pt-20">
  <!-- Add to your <head>: <link href='https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap' rel='stylesheet'> -->
  <div class="flex-1 flex flex-col items-start justify-center text-left max-w-lg md:max-w-md">
    <h1 class="text-4xl md:text-5xl font-extrabold mb-3" style="color: #2D3732;">
      Luisa Claussen
    </h1>
    <p class="text-lg md:text-xl font-semibold mb-2 text-[#768680]">Social Media Beratung & Strategie für lokale Unternehmen</p>
    <p class="text-base md:text-lg text-[#768680] max-w-md mb-6">Mehr Sichtbarkeit, mehr Kunden, mehr Erfolg – mit individueller Social Media Beratung, die wirklich zu Ihnen passt.</p>
    <div class="flex flex-col sm:flex-row gap-4">
      <button on:click={() => document.getElementById('calendly-section')?.scrollIntoView({ behavior: 'smooth' })}
        class="bg-[#768680] hover:bg-[#5e6b63] text-white font-bold py-3 px-8 rounded-full shadow-lg transition-all">
        Jetzt kostenloses Erstgespräch buchen
      </button>
      <button on:click={() => document.getElementById('about-section')?.scrollIntoView({ behavior: 'smooth' })}
        class="bg-white border-2 border-[#768680] text-[#768680] font-bold py-3 px-8 rounded-full shadow-md hover:bg-[#e9e5dc] transition-all">
        Mehr erfahren
      </button>
    </div>
  </div>
  <div class="flex-1 flex justify-center md:justify-end items-center mt-8 md:mt-0">
    <img src="/assets/Luisa_Freigestellt.png" alt="Luisa Claussen" class="w-72 md:w-[32rem] h-auto object-contain drop-shadow-2xl" />
  </div>
</section> 