<script lang="ts">
  import Boxes from "../assets/Boxes.svelte";
  import CircleCheck from "../assets/CircleCheck.svelte";
  import FileText from "../assets/FileText.svelte";
  import DeliverableCard from "./DeliverableCard.svelte";
  import SectionHeading from "./SectionHeading.svelte";

  const items = [
    { title: "Reusable YAML Workflows", sub: "GitHub Actions / Azure DevOps scripts", asset: "asset_01.delivered", icon: FileText },
    { title: "OWASP Dependency-Track Dashboard", sub: "Centralized vulnerability monitoring", asset: "asset_02.delivered", icon: Boxes },
    { title: "CycloneDX SBOM Exporter", sub: "Automated artifact generation", asset: "asset_03.delivered", icon: FileText },
    { title: "Developer Runbook & Audit Report", sub: "Documentation for clients and auditors", asset: "asset_04.delivered", icon: CircleCheck }
  ];
</script>

<section id="deliverables" class="relative py-24 border-t border-slate-800/60">
  <div class="max-w-[90rem] mx-auto px-6 lg:px-10">
    <SectionHeading eyebrow="tangible assets" title="Tangible Deliverables You Will Own" />
    <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-5">{#each items as item}<DeliverableCard {...item} />{/each}</div>
  </div>
</section>
