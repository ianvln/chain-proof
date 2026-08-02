<script lang="ts">
  import Boxes from "../../../assets/Boxes.svelte";
  import ChainProof from "../../../assets/ChainProof.svelte";
  import ShieldCheck from "../../../assets/ShieldCheck.svelte";
  import SectionHeading from "../../shared/SectionHeading.svelte";

  const pains = [
    { title: "Increasing NIS2 Pressure", body: "Enterprise clients and auditors demand proof of software supply chain security and CycloneDX SBOMs.", icon: ShieldCheck },
    { title: "Unknown Vulnerabilities", body: "Legacy NuGet packages and container base images often hide critical CVEs that go unnoticed.", icon: ChainProof },
    { title: "Developer Friction", body: "Dev teams are focused on feature delivery and don't have the bandwidth to set up AppSec tooling from scratch.", icon: Boxes }
  ];
</script>

<section class="relative py-24 border-t border-slate-800/60">
  <div class="max-w-[90rem] mx-auto px-6 lg:px-10">
    <SectionHeading eyebrow="the problem" title="Is Your Software Ready for Enterprise Security Audits?" />
    <div class="grid md:grid-cols-3 gap-5">
      {#each pains as pain, index}
        <article class="group relative p-6 rounded-xl border border-slate-800 bg-slate-900/40 backdrop-blur-sm hover:border-red-500/30 transition-colors">
          <div class="absolute top-0 left-0 w-full h-px bg-gradient-to-r from-transparent via-slate-700 to-transparent"></div>
          <div class="w-11 h-11 rounded-lg bg-slate-800/80 border border-slate-700 flex items-center justify-center mb-5"><pain.icon class="w-5 h-5 text-red-400" /></div>
          <h3 class="text-lg font-bold text-slate-100 mb-2.5">{pain.title}</h3>
          <p class="text-sm text-slate-400 leading-relaxed">{pain.body}</p>
          <span class="absolute bottom-4 right-4 font-mono text-[10px] text-slate-700 group-hover:text-slate-600">{String(index + 1).padStart(2, "0")}</span>
        </article>
      {/each}
    </div>
  </div>
</section>
