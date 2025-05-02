<script lang="ts">
  let active = 'Home';
  let mobileOpen = false;
  const navItems = [
    { name: 'Home', href: '/' },
    { name: 'About', href: '#about-section' },
    { name: 'Leistungen', href: '#services-section' },
    { name: 'Kontakt', href: '#calendly-section' }
  ];

  function handleSmoothScroll(event: MouseEvent, href: string, name: string) {
    if (href.startsWith('#')) {
      event.preventDefault();
      const el = document.querySelector(href);
      if (el) {
        el.scrollIntoView({ behavior: 'smooth' });
        active = name;
        mobileOpen = false;
      }
    }
  }
</script>

<nav class="flex justify-center sticky top-0 z-50 w-full">
  <!-- Desktop Navigation -->
  <div class="hidden md:flex bg-white border border-gray-200 rounded-full shadow-xl px-2 py-1 gap-2 md:gap-6 relative" style="box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.07);">
    {#each navItems as item}
      {#if item.name === 'Home'}
        <a
          href={item.href}
          class="relative flex items-center justify-center px-7 py-3 font-semibold text-gray-800 transition-colors duration-200 rounded-full"
          style="z-index:1;"
        >
          {#if active === item.name}
            <span class="absolute left-0 top-0 w-full h-full bg-gray-100 rounded-full z-0"></span>
          {/if}
          <span class="relative z-10">{item.name}</span>
        </a>
      {:else}
        <a
          href={item.href}
          class="relative flex items-center justify-center px-7 py-3 font-semibold text-gray-800 transition-colors duration-200 rounded-full"
          on:click={(e) => handleSmoothScroll(e, item.href, item.name)}
          style="z-index:1;"
        >
          {#if active === item.name}
            <span class="absolute left-0 top-0 w-full h-full bg-gray-100 rounded-full z-0"></span>
          {/if}
          <span class="relative z-10">{item.name}</span>
        </a>
      {/if}
    {/each}
  </div>

  <!-- Mobile Navigation -->
  <div class="flex md:hidden w-full justify-end pr-4">
    <button class="p-3 focus:outline-none" aria-label="Menü öffnen" on:click={() => mobileOpen = !mobileOpen}>
      <svg class="w-7 h-7 text-[#768680]" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
      </svg>
    </button>
    {#if mobileOpen}
      <div class="absolute top-16 right-4 bg-white border border-gray-200 rounded-2xl shadow-2xl flex flex-col w-56 z-50 animate-fade-in">
        {#each navItems as item}
          <a
            href={item.href}
            class="px-6 py-4 font-semibold text-gray-800 hover:bg-[#e9e5dc] rounded-2xl transition-colors duration-200"
            on:click={(e) => handleSmoothScroll(e, item.href, item.name)}
          >
            {item.name}
          </a>
        {/each}
      </div>
    {/if}
  </div>
</nav>

<style>
  html { scroll-behavior: smooth; }
  nav a {
    overflow: visible;
  }
  nav a span.absolute {
    box-shadow: none;
    transition: background 0.2s;
    display: block;
  }
  @keyframes fade-in {
    from { opacity: 0; transform: translateY(-10px); }
    to { opacity: 1; transform: translateY(0); }
  }
  .animate-fade-in {
    animation: fade-in 0.2s ease;
  }
</style> 