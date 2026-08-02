<script lang="ts">
  import Boxes from "../assets/Boxes.svelte";
  import FileText from "../assets/FileText.svelte";
  import GitBranch from "../assets/GitBranch.svelte";
  import ShieldCheck from "../assets/ShieldCheck.svelte";
  import RoadmapStep from "./RoadmapStep.svelte";
  import SectionHeading from "./SectionHeading.svelte";

  const steps = [
    { day: "DAY 1", title: "Discovery & Codebase Healthcheck", icon: FileText, points: ["Kick-off call with your engineering team.", "Deep-dive audit of your current CI/CD pipelines, .NET solution, NuGet packages, and Dockerfiles."], output: "Baseline Security Health Report & Action Plan.", code: "$ nexus-sec scan --solution ./src/\n> analyzing 142 NuGet packages\n> 3 Dockerfiles inspected\n> baseline report generated ✓" },
    { day: "DAY 2", title: "Pipeline Security Integration", icon: GitBranch, points: ["Integration of automated static code analysis (SonarQube) in GitHub Actions or Azure DevOps.", "Setup of Trivy container image and Dockerfile misconfiguration scanning."], output: "Fully automated security scans triggering on every Git Push & Pull Request.", code: "steps:\n  - name: SonarQube SAST\n    run: dotnet sonarscanner\n  - name: Trivy scan\n    run: trivy image app:latest" },
    { day: "DAY 3", title: "Software Supply Chain & SBOM Automation", icon: FileText, points: ["Automated generation of machine-readable CycloneDX SBOMs (Software Bill of Materials).", "API connection to a centralized OWASP Dependency-Track dashboard for 24/7 vulnerability monitoring."], output: "Real-time tracking of open-source vulnerabilities (CVEs) across all environments.", code: "$ nexus-sec sbom --format cyclonedx\n> components indexed\n> Dependency-Track upload complete ✓" },
    { day: "DAY 4", title: "Policy Tuning & Triage", icon: Boxes, points: ["Tune security policies to your risk profile and development workflow.", "Establish clear triage rules for vulnerabilities and actionable developer feedback."], output: "Security gates that protect production without blocking healthy delivery.", code: "$ nexus-sec policy apply\n> severity thresholds configured\n> triage workflow enabled ✓" },
    { day: "DAY 5", title: "Handover & Audit Readiness", icon: ShieldCheck, points: ["Walkthrough of the completed implementation with your engineering team.", "Deliver documentation, runbooks, and evidence for client and auditor review."], output: "Audit-ready proof to share with your clients, auditors, or CISO.", code: "$ nexus-sec attest --out report.pdf\n> NIS2 attestation signed ✓\n> ready for audit distribution" }
  ];
</script>

<section id="roadmap" class="relative py-24 border-t border-slate-800/60">
  <div class="absolute inset-0 grid-bg opacity-20"></div>
  <div class="relative max-w-[90rem] mx-auto px-6 lg:px-10">
    <SectionHeading eyebrow="the execution plan" title="The 5-Day DevSecOps Implementation Roadmap" description="A clear, transparent execution plan showing exactly how we transform your pipeline from zero to audit-ready." />
    <div class="max-w-4xl mx-auto">{#each steps as step}<RoadmapStep {...step} />{/each}</div>
  </div>
</section>
