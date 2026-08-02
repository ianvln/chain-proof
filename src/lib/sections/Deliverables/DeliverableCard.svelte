<script lang="ts">
  import type { Component } from "svelte";
  let { title, sub, asset, icon: Icon } = $props<{ title: string; sub: string; asset: string; icon: Component }>();
</script>

<article class="group relative p-6 rounded-xl border border-slate-800 bg-slate-900/40 backdrop-blur-sm hover:border-emerald-500/50 transition-all hover:-translate-y-1">
  <span class="absolute top-2 left-2 w-3 h-3 border-t border-l border-slate-700 group-hover:border-emerald-500/50"></span><span class="absolute top-2 right-2 w-3 h-3 border-t border-r border-slate-700 group-hover:border-emerald-500/50"></span><span class="absolute bottom-2 left-2 w-3 h-3 border-b border-l border-slate-700 group-hover:border-emerald-500/50"></span><span class="absolute bottom-2 right-2 w-3 h-3 border-b border-r border-slate-700 group-hover:border-emerald-500/50"></span>
  <div class="w-12 h-12 rounded-lg bg-slate-800/80 border border-slate-700 flex items-center justify-center mb-5 group-hover:bg-emerald-500/10 group-hover:border-emerald-500/40 transition-colors"><Icon class="w-5 h-5 text-blue-400 group-hover:text-emerald-400 transition-colors" /></div>
  <h3 class="text-base font-bold text-slate-100 leading-snug mb-1.5">{title}</h3>
  <p class="text-xs text-slate-500 font-mono">{sub}</p>
  <span class="mt-5 inline-block font-mono text-[10px] text-slate-700 group-hover:text-emerald-400/70 transition-colors">{asset}</span>
</article>
