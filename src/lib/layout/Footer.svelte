<script>
  import HomeButton from "./HomeButton.svelte";
</script>

<footer id="contact" class="relative border-t border-slate-800/60">
  <div class="border-t border-slate-800/60">
    <div class="max-w-[90rem] mx-auto px-6 lg:px-10 py-10">
      <div class="grid md:grid-cols-3 gap-8">
        <div>
          <HomeButton />
          <p class="text-sm text-slate-500 leading-relaxed">
            Turnkey DevSecOps &amp; NIS2 software supply chain security for .NET
            applications.
          </p>
        </div>
        <div>
          <div
            class="font-mono text-[11px] text-slate-600 uppercase tracking-widest mb-3"
          >
            /system-tree
          </div>
          <div class="">
            <div class="font-mono text-xs text-slate-500 py-0.5">root/</div>
            <div class="ml-3 border-l border-slate-800 pl-3">
              <div class="font-mono text-xs text-slate-500 py-0.5">
                services/
              </div>
              <div class="ml-3 border-l border-slate-800 pl-3">
                <div class="font-mono text-xs text-slate-500 py-0.5">audit</div>
              </div>
              <div class="ml-3 border-l border-slate-800 pl-3">
                <div class="font-mono text-xs text-slate-500 py-0.5">
                  sbom-automation
                </div>
              </div>
              <div class="ml-3 border-l border-slate-800 pl-3">
                <div class="font-mono text-xs text-slate-500 py-0.5">
                  pipeline-integration
                </div>
              </div>
            </div>
            <div class="ml-3 border-l border-slate-800 pl-3">
              <div class="font-mono text-xs text-slate-500 py-0.5">
                roadmap/
              </div>
            </div>
            <div class="ml-3 border-l border-slate-800 pl-3">
              <div class="font-mono text-xs text-slate-500 py-0.5">
                deliverables/
              </div>
            </div>
            <div class="ml-3 border-l border-slate-800 pl-3">
              <div class="font-mono text-xs text-slate-500 py-0.5">about/</div>
            </div>
          </div>
        </div>
        <div>
          <div
            class="font-mono text-[11px] text-slate-600 uppercase tracking-widest mb-3"
          >
            /status
          </div>
          <div class="space-y-1.5">
            <div
              class="flex items-center gap-2 font-mono text-xs text-slate-500"
            >
              <span class="w-1.5 h-1.5 bg-emerald-400 rounded-full"></span
              >pipeline: operational
            </div>
            <div
              class="flex items-center gap-2 font-mono text-xs text-slate-500"
            >
              <span class="w-1.5 h-1.5 bg-emerald-400 rounded-full"></span
              >compliance: NIS2-ready
            </div>
            <div
              class="flex items-center gap-2 font-mono text-xs text-slate-500"
            >
              <span class="w-1.5 h-1.5 bg-blue-400 rounded-full"></span>region:
              EU / Belgium
            </div>
          </div>
        </div>
      </div>
      <div
        class="mt-10 pt-6 border-t border-slate-800/60 flex flex-col sm:flex-row items-center justify-between gap-3"
      >
        <span class="font-mono text-[11px] text-slate-600"
          >© 2026 ChainProof · All rights reserved</span
        ><span class="font-mono text-[11px] text-slate-600"
          >build: stable · v2.0.0</span
        >
      </div>
    </div>
  </div>
</footer>
