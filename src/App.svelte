<script>
  import Deliverables from "./lib/sections/Deliverables/Deliverables.svelte";
  import Expert from "./lib/sections/Expert/Expert.svelte";
  import Header from "./lib/layout/Header.svelte";
  import Intro from "./lib/sections/Intro/Intro.svelte";
  import PainPoints from "./lib/sections/PainPoints/PainPoints.svelte";
  import Roadmap from "./lib/sections/Roadmap/Roadmap.svelte";
  import engiflex from "./assets/engiflex.png";
</script>

<Header />

<main>
  <Intro />
  <section
    data-source-location="src/components/Landing/PartnershipBadge.jsx:6:4"
    data-dynamic-content="false"
    class="relative py-16 border-t border-slate-800/60"
  >
    <div
      data-source-location="src/components/Landing/PartnershipBadge.jsx:7:6"
      data-dynamic-content="false"
      class="absolute inset-x-0 top-0 h-px bg-gradient-to-r from-transparent via-emerald-500/40 to-transparent"
    ></div>
    <div
      data-source-location="src/components/Landing/PartnershipBadge.jsx:8:6"
      data-dynamic-content="false"
      class="max-w-3xl mx-auto px-6 text-center"
    >
      <div
        data-source-location="src/components/Landing/PartnershipBadge.jsx:9:8"
        data-dynamic-content="false"
        class="relative inline-flex flex-col items-center gap-5 px-8 sm:px-12 py-8 rounded-2xl border border-slate-700 bg-slate-900/50 backdrop-blur-xl"
      >
        <div
          data-source-location="src/components/Landing/PartnershipBadge.jsx:11:10"
          data-dynamic-content="false"
          class="absolute -inset-4 bg-gradient-to-br from-emerald-500/10 via-blue-500/5 to-transparent rounded-3xl blur-2xl -z-10"
        ></div>
        <span
          data-source-location="src/components/Landing/PartnershipBadge.jsx:13:10"
          data-dynamic-content="false"
          class="font-mono text-[11px] text-slate-400 uppercase tracking-[0.3em]"
          >In Proud Partnership With</span
        >
        <div class="flex justify-center items-center gap-3">
          <img src={engiflex} alt="EngiFlex logo" width="40" height="40" />
          <p class="text-xl font-bold">EngiFlex</p>
        </div>
        <div
          data-source-location="src/components/Landing/PartnershipBadge.jsx:19:10"
          data-dynamic-content="false"
          class="flex items-center gap-2"
        >
          <span
            data-source-location="src/components/Landing/PartnershipBadge.jsx:20:12"
            data-dynamic-content="false"
            class="w-1.5 h-1.5 bg-emerald-400 rounded-full animate-pulse-dot"
          ></span><span
            data-source-location="src/components/Landing/PartnershipBadge.jsx:21:12"
            data-dynamic-content="false"
            class="font-mono text-[11px] text-slate-500"
            >powering flexible engineering together</span
          >
        </div>
      </div>
    </div>
  </section>
  <PainPoints />
  <Roadmap />
  <Deliverables />
  <Expert />
</main>
