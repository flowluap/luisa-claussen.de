<section id="calendly-section" class="py-16 flex flex-col items-center bg-white">
  <h2 class="text-2xl font-bold text-[#768680] mb-4 text-center" style="color: #e9e5dc;">Jetzt kostenloses 15-Minuten-Beratungsgespräch buchen</h2>
  <p class="text-[#768680] mb-8 text-center">Unverbindlich & persönlich – sichern Sie sich Ihren Termin!</p>
  <!-- Cal inline embed code begins -->
  <div style="width:100%;height:100%;overflow:scroll" id="my-cal-inline"></div>
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
</section> 