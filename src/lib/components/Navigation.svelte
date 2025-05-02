<script lang="ts">
  let active = 'Home';
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
      }
    }
  }
</script>

<nav class="flex justify-center sticky top-0 z-50 w-full">
  <div class="flex bg-white border border-gray-200 rounded-full shadow-xl px-2 py-1 gap-2 md:gap-6 relative" style="box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.07);">
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
</style> 