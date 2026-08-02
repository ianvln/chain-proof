<script>
  import HomeButton from "./HomeButton.svelte";
  import Navigation from "./Navigation.svelte";
</script>

<header
  class="fixed top-0 inset-x-0 z-50 transition-all duration-300 bg-transparent border-b border-transparent"
>
  <div class="max-w-[90rem] mx-auto px-6 lg:px-10">
    <div class="max-w-[90rem] mx-auto px-6 lg:px-10">
      <div class="flex items-center justify-between h-16">
        <HomeButton />
        <Navigation />
        <div>
          <button
            type="button"
            class="hidden md:inline-flex items-center px-4 py-2 rounded-md bg-emerald-500 text-slate-950 text-sm font-semibold hover:bg-emerald-400 transition-colors"
          >
            Book a call
          </button>
        </div>
      </div>
    </div>
  </div>
</header>
