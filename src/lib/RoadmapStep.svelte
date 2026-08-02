<script lang="ts">
  import type { Component } from "svelte";
  import type { SvelteComponent } from "svelte";

  let { day, title, points, output, code, icon: Icon } = $props<{
    day: string; title: string; points: string[]; output: string; code: string;
    icon: Component<SvelteComponent>;
  }>();
</script>

<article class="relative pl-16 lg:pl-24 transition-all duration-700">
  <span class="absolute left-[22px] top-12 bottom-0 w-px bg-gradient-to-b from-emerald-500/60 to-slate-800"></span>
  <div class="absolute left-0 top-0 flex items-center justify-center w-11 h-11 rounded-full bg-slate-900 border-2 border-emerald-500/60 z-10"><span class="w-2.5 h-2.5 bg-emerald-400 rounded-full animate-pulse-dot"></span></div>
  <div class="pb-16">
    <div class="flex items-center gap-3 mb-3"><span class="font-mono text-xs text-emerald-400 font-semibold tracking-wider">{day}</span><span class="h-px flex-1 bg-slate-800"></span><Icon class="w-4 h-4 text-blue-400" /></div>
    <h3 class="text-xl sm:text-2xl font-bold text-slate-50 mb-4">{title}</h3>
    <div class="grid lg:grid-cols-2 gap-5">
      <div>
        <ul class="space-y-2.5 mb-5">{#each points as point}<li class="flex gap-3 text-sm text-slate-400 leading-relaxed"><span class="text-emerald-400 mt-0.5 shrink-0">▹</span><span>{point}</span></li>{/each}</ul>
        <div class="inline-flex items-start gap-2 px-3 py-2 rounded-md bg-emerald-500/10 border border-emerald-500/20"><span class="font-mono text-[10px] text-emerald-400 font-semibold uppercase mt-0.5">Output</span><span class="text-xs text-emerald-100/90 leading-relaxed">{output}</span></div>
      </div>
      <div class="rounded-lg border border-slate-800 bg-slate-950/80 overflow-hidden">
        <div class="px-3 py-2 border-b border-slate-800 flex items-center gap-1.5"><span class="w-2 h-2 rounded-full bg-slate-700"></span><span class="w-2 h-2 rounded-full bg-slate-700"></span><span class="w-2 h-2 rounded-full bg-slate-700"></span><span class="ml-2 font-mono text-[10px] text-slate-600">terminal</span></div>
        <pre class="p-4 font-mono text-[11px] leading-relaxed text-slate-300 overflow-x-auto whitespace-pre"><code>{code}</code></pre>
      </div>
    </div>
  </div>
</article>
