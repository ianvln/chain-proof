<script lang="ts">
  import engiflex from "../../../assets/engiflex.png";
</script>

<section class="relative py-16 border-t border-slate-800/60">
  <div
    class="absolute inset-x-0 top-0 h-px from-transparent via-emerald-500/40 to-transparent"
  ></div>
  <div class="max-w-3xl mx-auto px-6 text-center">
    <div
      class="relative inline-flex flex-col items-center gap-5 px-8 sm:px-12 py-8 rounded-2xl border border-slate-700 bg-slate-900/50 backdrop-blur-xl"
    >
      <div
        class="absolute -inset-4 from-emerald-500/10 via-blue-500/5 to-transparent rounded-3xl blur-2xl -z-10"
      ></div>
      <span
        class="font-mono text-[11px] text-slate-400 uppercase tracking-[0.3em]"
        >In Proud Partnership With</span
      >
      <div class="flex justify-center items-center gap-3">
        <img src={engiflex} alt="EngiFlex logo" width="40" height="40" />
        <p class="text-xl font-bold">EngiFlex</p>
      </div>
      <div class="flex items-center gap-2">
        <span class="w-1.5 h-1.5 bg-emerald-400 rounded-full animate-pulse-dot"
        ></span>
        <span class="font-mono text-[11px] text-slate-500"
          >powering flexible engineering together</span
        >
      </div>
    </div>
  </div>
</section>
