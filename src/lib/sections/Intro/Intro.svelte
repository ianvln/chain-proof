<script lang="ts">
  import ArrowRight from "../../../assets/ArrowRight.svelte";
  import { contact } from "../../config/contact";
  import SecurityPipeline from "./SecurityPipeline.svelte";
  import Calendar from "../../../assets/Calendar.svelte";
</script>

<section class="relative overflow-hidden pt-32 pb-24 lg:pt-40 lg:pb-32">
  <div class="absolute inset-0 grid-bg opacity-40"></div>
  <div
    class="absolute inset-0 bg-gradient-to-b from-slate-950 via-transparent to-slate-950"
  ></div>
  <div
    class="absolute top-0 left-1/4 w-[40rem] h-[40rem] bg-emerald-500/10 rounded-full blur-[120px]"
  ></div>
  <div
    class="absolute bottom-0 right-1/4 w-[36rem] h-[36rem] bg-blue-500/10 rounded-full blur-[120px]"
  ></div>
  <div class="relative max-w-[90rem] mx-auto px-6 lg:px-10">
    <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
      <div>
        <div
          class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-slate-900/80 border border-slate-800 mb-6"
        >
          <span
            class="w-1.5 h-1.5 bg-emerald-400 rounded-full animate-pulse-dot"
          ></span>
          <span class="font-mono text-xs text-slate-300"
            >For .NET &amp; Cloud Development Teams</span
          >
        </div>
        <h1
          class="text-4xl sm:text-5xl lg:text-6xl font-black tracking-tight text-slate-50 leading-[1.05]"
        >
          Automate Your Software Security &amp; <span
            class="text-emerald-400 text-glow-emerald">NIS2 Compliance</span
          > in 5 Days
        </h1>
        <p class="mt-6 text-lg text-slate-400 leading-relaxed max-w-xl">
          Stop worrying about client security audits. We integrate automated
          SAST, SBOM generation, and container scanning directly into your
          GitHub or Azure DevOps pipelines—without slowing down your developers.
        </p>
        <div class="mt-8 flex flex-col sm:flex-row gap-3">
          <a href={`mailto:${contact.email}`} class="button-primary"
            ><Calendar class="lucide lucide-calendar w-4.5 h-4.5" />Schedule a
            call</a
          >
          <a
            href="#roadmap"
            class="inline-flex items-center justify-center gap-2 px-6 py-3.5 rounded-lg border border-slate-700 text-slate-200 font-semibold hover:border-emerald-500/50 hover:text-emerald-400 transition-colors"
          >
            Explore the 5-Day Roadmap <ArrowRight
              class="lucide lucide-arrow-right w-4 h-4"
            />
          </a>
        </div>
        <div class="mt-10 flex items-center gap-6 text-sm text-slate-500">
          <div class="flex items-center gap-2">
            <span class="font-mono text-emerald-400 font-semibold">5 days</span
            ><span>to audit-ready</span>
          </div>
          <div class="w-px h-4 bg-slate-800"></div>
          <div class="flex items-center gap-2">
            <span class="font-mono text-blue-400 font-semibold">Zero</span><span
              >developer slowdown</span
            >
          </div>
        </div>
      </div>
      <SecurityPipeline />
    </div>
  </div>
</section>
