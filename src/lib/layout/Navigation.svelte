<script lang="ts">
  import { contact } from "../config/contact";

  let menuOpen = $state(false);

  const links = [
    { href: "#roadmap", label: "Roadmap" },
    { href: "#deliverables", label: "Deliverables" },
    { href: "#expert", label: "Expert" },
  ];
</script>

<nav aria-label="Main navigation">
  <div class="hidden md:flex items-center gap-8">
    {#each links as link}
      <a
        href={link.href}
        class="text-sm text-slate-300 hover:text-emerald-400 transition-colors font-medium"
      >{link.label}</a>
    {/each}
  </div>

  <div class="md:hidden relative">
    <button
      type="button"
      class="inline-flex items-center justify-center w-10 h-10 rounded-md text-slate-200 hover:bg-slate-800/80 transition-colors"
      aria-label={menuOpen ? "Close navigation menu" : "Open navigation menu"}
      aria-expanded={menuOpen}
      aria-controls="mobile-navigation"
      onclick={() => (menuOpen = !menuOpen)}
    >
      <span class="sr-only">Menu</span>
      {#if menuOpen}
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" class="w-5 h-5" aria-hidden="true">
          <path d="M6 6l12 12M18 6L6 18" stroke-linecap="round" />
        </svg>
      {:else}
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" class="w-5 h-5" aria-hidden="true">
          <path d="M4 6h16M4 12h16M4 18h16" stroke-linecap="round" />
        </svg>
      {/if}
    </button>

    {#if menuOpen}
      <div
        id="mobile-navigation"
        class="absolute right-0 top-12 w-56 rounded-lg border border-slate-800 bg-slate-950/95 p-2 shadow-xl backdrop-blur-xl"
      >
        {#each links as link}
          <a
            href={link.href}
            class="block rounded-md px-3 py-2.5 text-sm font-medium text-slate-200 hover:bg-slate-800 hover:text-emerald-400 transition-colors"
            onclick={() => (menuOpen = false)}
          >{link.label}</a>
        {/each}
        <a
          href={`mailto:${contact.email}`}
          class="mt-2 block rounded-md bg-emerald-500 px-3 py-2.5 text-center text-sm font-semibold text-slate-950 hover:bg-emerald-400 transition-colors"
          onclick={() => (menuOpen = false)}
        >Book a call</a>
      </div>
    {/if}
  </div>
</nav>
