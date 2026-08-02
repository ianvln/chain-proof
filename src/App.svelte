<script>
  import ArrowRight from "./assets/ArrowRight.svelte";
  import Calendar from "./assets/Calendar.svelte";
  import Background from "./lib/Background.svelte";
  import Deliverables from "./lib/Deliverables.svelte";
  import Expert from "./lib/Expert.svelte";
  import Header from "./lib/Header.svelte";
  import PainPoints from "./lib/PainPoints.svelte";
  import Roadmap from "./lib/Roadmap.svelte";
  import SecurityPipeline from "./lib/SecurityPipeline.svelte";
</script>

<Header />

<main>
  <Background>
    <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
      <div>
        <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-slate-900/80 border border-slate-800 mb-6">
          <span class="w-1.5 h-1.5 bg-emerald-400 rounded-full animate-pulse-dot"></span>
          <span class="font-mono text-xs text-slate-300">For .NET &amp; Cloud Development Teams</span>
        </div>
        <h1 class="text-4xl sm:text-5xl lg:text-6xl font-black tracking-tight text-slate-50 leading-[1.05]">
          Automate Your Software Security &amp; <span class="text-emerald-400 text-glow-emerald">NIS2 Compliance</span> in 5 Days
        </h1>
        <p class="mt-6 text-lg text-slate-400 leading-relaxed max-w-xl">
          Stop worrying about client security audits. We integrate automated SAST, SBOM generation, and container scanning directly into your GitHub or Azure DevOps pipelines—without slowing down your developers.
        </p>
        <div class="mt-8 flex flex-col sm:flex-row gap-3">
          <button type="button" class="button-primary"><Calendar class="lucide lucide-calendar w-4.5 h-4.5" />Schedule a call</button>
          <a href="#roadmap" class="inline-flex items-center justify-center gap-2 px-6 py-3.5 rounded-lg border border-slate-700 text-slate-200 font-semibold hover:border-emerald-500/50 hover:text-emerald-400 transition-colors">
            Explore the 5-Day Roadmap <ArrowRight class="lucide lucide-arrow-right w-4 h-4" />
          </a>
        </div>
        <div class="mt-10 flex items-center gap-6 text-sm text-slate-500">
          <div class="flex items-center gap-2"><span class="font-mono text-emerald-400 font-semibold">5 days</span><span>to audit-ready</span></div>
          <div class="w-px h-4 bg-slate-800"></div>
          <div class="flex items-center gap-2"><span class="font-mono text-blue-400 font-semibold">Zero</span><span>developer slowdown</span></div>
        </div>
      </div>
      <SecurityPipeline />
    </div>
  </Background>

  <PainPoints />
  <Roadmap />
  <Deliverables />
  <Expert />
</main>
