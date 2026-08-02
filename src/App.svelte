<script>
  import viteLogo from './assets/vite.svg'
  import heroImg from './assets/hero.png'
  import Header from './lib/Header.svelte'
  import Background from './lib/Background.svelte'
  import SecurityPipeline from './lib/SecurityPipeline.svelte'
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
          <h1 class="text-4xl sm:text-5xl lg:text-6xl font-black tracking-tight text-slate-50 leading-[1.05]">Automate Your Software Security &amp; <span class="text-emerald-400 text-glow-emerald">NIS2 Compliance</span> in 5 Days</h1>
          <p class="mt-6 text-lg text-slate-400 leading-relaxed max-w-xl">Stop worrying about client security audits. We integrate automated SAST, SBOM generation, and container scanning directly into your GitHub or Azure DevOps pipelines—without slowing down your developers.</p>
          <div class="mt-8 flex flex-col sm:flex-row gap-3"><a href="#contact" class="inline-flex items-center justify-center gap-2 px-6 py-3.5 rounded-lg bg-emerald-500 text-slate-950 font-semibold hover:bg-emerald-400 transition-colors glow-emerald">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-calendar w-4.5 h-4.5"><path d="M8 2v4"></path><path d="M16 2v4"></path><rect width="18" height="18" x="3" y="4" rx="2"></rect><path d="M3 10h18"></path></svg>Schedule a Free DevSecOps Audit Call</a><a href="#roadmap" class="inline-flex items-center justify-center gap-2 px-6 py-3.5 rounded-lg border border-slate-700 text-slate-200 font-semibold hover:border-emerald-500/50 hover:text-emerald-400 transition-colors">Explore the 5-Day Roadmap<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-arrow-right w-4 h-4"><path d="M5 12h14"></path><path d="m12 5 7 7-7 7"></path></svg></a><svg class="h-9 w-auto self-center opacity-90 sm:ml-2" viewBox="0 0 214 48" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="EngiFlex — Flexible in Engineering"><defs><linearGradient id="engiflex-grad" x1="8" y1="8" x2="40" y2="40" gradientUnits="userSpaceOnUse"><stop offset="0" stop-color="#A855F7"></stop><stop offset="0.5" stop-color="#3B82F6"></stop><stop offset="1" stop-color="#10B981"></stop></linearGradient></defs><path d="M8,14 L8,34 Q8,40 13.36,37.32 L34.64,26.68 Q40,24 34.64,21.32 L13.36,10.68 Q8,8 8,14 Z" fill="url(#engiflex-grad)"></path><path d="M10.77,15.16 L10.77,32.84 Q10.77,35.84 13.47,34.52 L32.31,25.32 Q35.01,24 32.31,22.68 L13.47,13.48 Q10.77,12.16 10.77,15.16 Z" fill="#0F172A"></path><text x="50" y="27" fill="#FFFFFF" font-family="Inter, ui-sans-serif, system-ui, sans-serif" font-size="20" font-weight="800" letter-spacing="-0.5">EngiFlex</text><text x="50" y="40" fill="#FFFFFF" font-family="Inter, ui-sans-serif, system-ui, sans-serif" font-size="6.5" font-weight="600" letter-spacing="2">FLEXIBLE IN ENGINEERING</text></svg></div><div class="mt-10 flex items-center gap-6 text-sm text-slate-500"><div class="flex items-center gap-2"><span class="font-mono text-emerald-400 font-semibold">5 days</span><span>to audit-ready</span></div><div class="w-px h-4 bg-slate-800"></div><div class="flex items-center gap-2"><span class="font-mono text-blue-400 font-semibold">Zero</span><span>developer slowdown</span></div></div></div>
      <SecurityPipeline />
    </div>
  </Background>
</main>

<section id="center">
  <div class="hero">
    <img src={heroImg} class="base" width="170" height="179" alt="" />
    <img src={viteLogo} class="vite" alt="Vite logo" />
  </div>
  <div>
    <h1>Get started</h1>
    <p>Edit <code>src/App.svelte</code> and save to test <code>HMR</code></p>
  </div>
</section>

<div class="ticks"></div>
<section id="spacer"></section>
