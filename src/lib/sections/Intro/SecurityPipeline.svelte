<script>
  import GitBranch from "../../../assets/GitBranch.svelte";
  import ShieldCheck from "../../../assets/ShieldCheck.svelte";
  import Boxes from "../../../assets/Boxes.svelte";
  import FileText from "../../../assets/FileText.svelte";
  import CircleCheck from "../../../assets/CircleCheck.svelte";
</script>

<div class="relative">
  <div class="relative">
    <div
      class="absolute -inset-4 bg-gradient-to-br from-emerald-500/10 via-blue-500/5 to-transparent rounded-2xl blur-2xl"
    ></div>
    <div
      class="relative rounded-xl border border-slate-700/80 bg-slate-900/80 backdrop-blur-xl overflow-hidden shadow-2xl"
    >
      <div
        class="flex items-center justify-between px-4 py-3 border-b border-slate-800 bg-slate-950/60"
      >
        <div class="flex items-center gap-2">
          <span class="w-3 h-3 rounded-full bg-red-500/80"></span><span
            class="w-3 h-3 rounded-full bg-amber-400/80"
          ></span><span class="w-3 h-3 rounded-full bg-emerald-500/80"
          ></span><span class="ml-3 font-mono text-xs text-slate-500"
            >.github/workflows/security.yml</span
          >
        </div>
        <div class="flex items-center gap-2">
          <span
            class="w-1.5 h-1.5 bg-emerald-400 rounded-full animate-pulse-dot"
          ></span>
          <span class="font-mono text-[11px] text-emerald-400">RUNNING</span>
        </div>
      </div>
      <div class="p-5 space-y-3">
        <div
          class="font-mono text-[11px] text-slate-500 mb-2 flex items-center justify-between"
        >
          <span>workflow / dotnet-security</span><span class="text-emerald-400"
            >● compliance: passed</span
          >
        </div>
        <div
          class="flex items-center gap-3 p-3 rounded-lg bg-slate-950/50 border border-slate-800 hover:border-emerald-500/40 transition-colors group"
        >
          <GitBranch
            class="lucide lucide-git-branch w-4 h-4 text-blue-400 shrink-0"
          />
          <div class="flex-1 min-w-0">
            <div class="font-mono text-sm text-slate-200">git push</div>
          </div>
          <span class="font-mono text-[10px] text-slate-500 hidden sm:inline"
            >main</span
          >
          <div class="flex items-center gap-1.5 text-emerald-400">
            <CircleCheck class="lucide lucide-circle-check w-4 h-4" />
            <span class="font-mono text-[11px] font-medium uppercase"
              >passed</span
            >
          </div>
        </div>
        <div
          class="flex items-center gap-3 p-3 rounded-lg bg-slate-950/50 border border-slate-800 hover:border-emerald-500/40 transition-colors group"
        >
          <ShieldCheck
            class="lucide lucide-shield-check w-4 h-4 text-blue-400 shrink-0"
          />
          <div class="flex-1 min-w-0">
            <div class="font-mono text-sm text-slate-200">SonarQube SAST</div>
          </div>
          <span class="font-mono text-[10px] text-slate-500 hidden sm:inline"
            >0 criticals</span
          >
          <div class="flex items-center gap-1.5 text-emerald-400">
            <CircleCheck class="lucide lucide-circle-check w-4 h-4" />
            <span class="font-mono text-[11px] font-medium uppercase"
              >passed</span
            >
          </div>
        </div>
        <div
          class="flex items-center gap-3 p-3 rounded-lg bg-slate-950/50 border border-slate-800 hover:border-emerald-500/40 transition-colors group"
        >
          <Boxes class="lucide lucide-boxes w-4 h-4 text-blue-400 shrink-0" />
          <div class="flex-1 min-w-0">
            <div class="font-mono text-sm text-slate-200">
              Trivy Container Scan
            </div>
          </div>
          <span class="font-mono text-[10px] text-slate-500 hidden sm:inline"
            >0 HIGH</span
          >
          <div class="flex items-center gap-1.5 text-emerald-400">
            <CircleCheck class="lucide lucide-circle-check w-4 h-4" />
            <span class="font-mono text-[11px] font-medium uppercase"
              >passed</span
            >
          </div>
        </div>
        <div
          class="flex items-center gap-3 p-3 rounded-lg bg-slate-950/50 border border-slate-800 hover:border-emerald-500/40 transition-colors group"
        >
          <FileText
            class="lucide lucide-file-text w-4 h-4 text-blue-400 shrink-0"
          />
          <div class="flex-1 min-w-0">
            <div class="font-mono text-sm text-slate-200">CycloneDX SBOM</div>
          </div>
          <span class="font-mono text-[10px] text-slate-500 hidden sm:inline"
            >exported</span
          >
          <div class="flex items-center gap-1.5 text-emerald-400">
            <CircleCheck class="lucide lucide-circle-check w-4 h-4" />
            <span class="font-mono text-[11px] font-medium uppercase"
              >passed</span
            >
          </div>
        </div>
      </div>
      <div
        class="px-5 py-3 border-t border-slate-800 bg-slate-950/60 flex items-center justify-between"
      >
        <span class="font-mono text-[11px] text-slate-400"
          >build #482 · main · 2m 14s</span
        >
        <div
          class="flex items-center gap-2 px-2.5 py-1 rounded-md bg-emerald-500/10 border border-emerald-500/30"
        >
          <ShieldCheck
            class="lucide lucide-shield-check w-3.5 h-3.5 text-emerald-400"
          />
          <span class="font-mono text-[11px] text-emerald-400 font-semibold"
            >AUDIT-READY</span
          >
        </div>
      </div>
    </div>
  </div>
</div>
