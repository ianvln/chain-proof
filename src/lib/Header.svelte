<script>
  import ChainProofLogo from "../assets/ChainProof.svelte";
  import Navigation from "./Navigation.svelte";
</script>

<header
  class="fixed top-0 inset-x-0 z-50 transition-all duration-300 bg-transparent border-b border-transparent"
>
  <div class="max-w-[90rem] mx-auto px-6 lg:px-10">
    <div class="max-w-[90rem] mx-auto px-6 lg:px-10">
      <div class="flex items-center justify-between h-16">
        <a href="/" class="flex items-center gap-2.5 group">
          <ChainProofLogo
            class="w-6 h-6 text-emerald-400"
            aria-label="ChainProof logo"
          />
          <span
            class="absolute -top-0.5 -right-0.5 w-1.5 h-1.5 bg-emerald-400 rounded-full animate-pulse-dot"
          ></span>
          <span
            class="font-mono text-sm font-bold tracking-tight text-slate-100"
            >Chain<span class="text-emerald-400">Proof</span>
          </span>
        </a>
        <Navigation />
      </div>
    </div>
  </div>
</header>
