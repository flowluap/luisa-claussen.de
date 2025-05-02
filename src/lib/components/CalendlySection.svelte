<script lang="ts">
  let activeTab = 0;
  const tabs = [
    { label: 'Termin buchen' },
    { label: 'Kontakt' }
  ];
</script>

<section id="calendly-section" class="py-16 flex flex-col items-center bg-white w-full">
  <h2 class="text-2xl font-bold mb-4 text-center" style="color: #2D3732;">Jetzt kostenloses 15-Minuten-Beratungsgespräch buchen</h2>
  <p class="text-[#768680] mb-8 text-center">Unverbindlich & persönlich – sichern Sie sich Ihren Termin!</p>

  <!-- Tabs -->
  <div class="flex justify-center mb-8 w-full">
    <div class="inline-flex rounded-full bg-[#e9e5dc] p-1 shadow-md">
      {#each tabs as tab, i}
        <button
          class="px-6 py-2 rounded-full font-semibold focus:outline-none transition-colors duration-200 text-sm md:text-base"
          class:bg-white={activeTab === i}
          class:text-[#2D3732]={activeTab === i}
          class:text-[#768680]={activeTab !== i}
          class:shadow={activeTab === i}
          on:click={() => activeTab = i}
        >
          {tab.label}
        </button>
      {/each}
    </div>
  </div>

  <!-- Tab Content Wrapper with fixed min-height to prevent jump -->
  <div class="relative w-full flex justify-center min-h-[420px]">
    {#if activeTab === 0}
      <!-- Cal inline embed code begins -->
      <div class="absolute inset-0 flex justify-center items-start">
        <div style="width:100%;height:400px;overflow:scroll" id="my-cal-inline"></div>
      </div>
      <script type="text/javascript">
        (function (C, A, L) { let p = function (a, ar) { a.q.push(ar); }; let d = C.document; C.Cal = C.Cal || function () { let cal = C.Cal; let ar = arguments; if (!cal.loaded) { cal.ns = {}; cal.q = cal.q || []; d.head.appendChild(d.createElement("script")).src = A; cal.loaded = true; } if (ar[0] === L) { const api = function () { p(api, arguments); }; const namespace = ar[1]; api.q = api.q || []; if(typeof namespace === "string"){cal.ns[namespace] = cal.ns[namespace] || api;p(cal.ns[namespace], ar);p(cal, ["initNamespace", namespace]);} else p(cal, ar); return;} p(cal, ar); }; })(window, "https://app.cal.com/embed/embed.js", "init");
        Cal("init", "15min", {origin:"https://cal.com"});

        Cal.ns["15min"]("inline", {
          elementOrSelector:"#my-cal-inline",
          config: {"layout":"month_view","theme":"light"},
          calLink: "luisa-claussen/15min",
        });

        Cal.ns["15min"]("ui", {"theme":"light","cssVarsPerTheme":{"light":{"cal-brand":"#768680"},"dark":{"cal-brand":"#768680"}},"hideEventTypeDetails":false,"layout":"month_view"});
      </script>
      <!-- Cal inline embed code ends -->
    {:else}
      <div class="absolute inset-0 flex flex-col items-center justify-center w-full max-w-md mx-auto rounded-2xl p-8 shadow-md min-h-[400px]">
        <div class="mb-4 text-[#768680] text-lg font-semibold">Kontaktinformationen</div>
        <div class="flex flex-col items-center gap-2">
          <a href="mailto:info@luisa-claussen.de" class="text-[#2D3732] font-bold underline text-lg">info@luisa-claussen.de</a>
          <span class="text-[#768680] text-base">Luisa Claußen</span>
        </div>
      </div>
    {/if}
  </div>
</section> 