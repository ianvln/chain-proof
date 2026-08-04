<script lang="ts">
  import { onMount } from "svelte";
  import { contact } from "../config/contact";
  import HomeButton from "./HomeButton.svelte";
  import Navigation from "./Navigation.svelte";

  let isScrolled = $state(false);

  onMount(() => {
    const updateScrollState = () => {
      isScrolled = window.scrollY > 0;
    };

    updateScrollState();
    window.addEventListener("scroll", updateScrollState, { passive: true });

    return () => window.removeEventListener("scroll", updateScrollState);
  });
</script>

<header
  class={`fixed top-0 inset-x-0 z-50 transition-all duration-300 ${
    isScrolled
      ? "backdrop-blur-xl bg-slate-950/70 border-b border-slate-800/80"
      : "bg-transparent border-b border-transparent"
  }`}
>
  <div class="max-w-[90rem] mx-auto px-4 sm:px-6 lg:px-10">
    <div class="flex items-center justify-between h-16">
      <HomeButton />
      <Navigation />
      <a
        href={`mailto:${contact.email}`}
        class="hidden md:inline-flex items-center px-4 py-2 rounded-md bg-emerald-500 text-slate-950 text-sm font-semibold hover:bg-emerald-400 transition-colors"
      >
        Book a call
      </a>
    </div>
  </div>
</header>
