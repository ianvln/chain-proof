<script lang="ts">
  import headshot from "../../../assets/headshot.jpg";
  import ShieldCheck from "../../../assets/ShieldCheck.svelte";
  const stack = [
    "C#",
    "ASP.NET",
    "Java",
    "Spring Boot",
    "OpenShift",
    "Kubernetes",
    "Docker",
    "SonarQube",
    "Trivy",
    "GitHub Actions",
    "Azure DevOps",
  ];
</script>

<section id="expert" class="relative py-24 border-t border-slate-800/60">
  <div
    class="absolute top-1/2 left-0 w-[30rem] h-[30rem] bg-blue-500/5 rounded-full blur-[120px] -translate-y-1/2"
  ></div>
  <div class="relative max-w-[90rem] mx-auto px-6 lg:px-10">
    <div class="grid lg:grid-cols-5 gap-10 lg:gap-16 items-center">
      <div class="lg:col-span-2">
        <div class="relative max-w-sm mx-auto">
          <div
            class="absolute -inset-3 bg-gradient-to-br from-emerald-500/15 to-blue-500/10 rounded-2xl blur-xl"
          ></div>
          <div
            class="relative rounded-2xl border border-slate-700 bg-slate-900/60 backdrop-blur-xl overflow-hidden"
          >
            <div class="relative aspect-square">
              <img
                src={headshot}
                loading="lazy"
                class="w-full h-full inset-0 absolute object-cover"
                alt="Ian Vermeulen, Senior Software Engineer &amp; AppSec Specialist"
              />
              <div
                class="absolute inset-0 bg-gradient-to-t from-slate-950 via-slate-950/20 to-transparent"
              ></div>
              <div
                class="absolute top-3 left-3 right-3 flex items-center justify-between"
              >
                <div
                  class="flex items-center gap-1.5 px-2 py-1 rounded bg-slate-950/80 backdrop-blur border border-emerald-500/30"
                >
                  <ShieldCheck class="w-3 h-3 text-emerald-400" /><span
                    class="font-mono text-[9px] text-emerald-400 font-semibold uppercase"
                    >Cleared</span
                  >
                </div>
                <span class="font-mono text-[9px] text-slate-400"
                  >ID: NXS-001</span
                >
              </div>
              <div class="absolute bottom-0 inset-x-0 p-4">
                <div
                  class="font-mono text-[10px] text-emerald-400 uppercase tracking-widest mb-0.5"
                >
                  AppSec Specialist
                </div>
                <div class="text-xl font-bold text-slate-50">Ian Vermeulen</div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="lg:col-span-3">
        <span
          class="font-mono text-xs text-emerald-400 uppercase tracking-widest"
          >// the architect</span
        >
        <h2
          class="mt-3 text-3xl sm:text-4xl font-black tracking-tight text-slate-50"
        >
          Architected by Enterprise Security Specialist
        </h2>
        <p class="mt-5 text-lg text-slate-300 leading-relaxed">
          <span class="text-emerald-400 font-semibold">Ian Vermeulen</span>,
          Senior Software Engineer &amp; AppSec Specialist.
        </p>
        <p class="mt-4 text-slate-400 leading-relaxed">
          Ex-KPMG Advisory background combined with hands-on critical
          infrastructure development in multiple environments.
        </p>
        <div class="mt-8">
          <div
            class="font-mono text-[11px] text-slate-500 uppercase tracking-widest mb-3"
          >
            Verified Tech Stack
          </div>
          <div class="flex flex-wrap gap-2">
            {#each stack as technology}<span
                class="px-3 py-1.5 rounded-md bg-slate-900/80 border border-slate-700 hover:border-emerald-500/40 transition-colors font-mono text-xs text-slate-300"
                >{technology}</span
              >{/each}
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
