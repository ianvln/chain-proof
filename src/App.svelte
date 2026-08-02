<script>
  import Deliverables from "./lib/Deliverables.svelte";
  import Expert from "./lib/Expert.svelte";
  import Header from "./lib/Header.svelte";
  import PainPoints from "./lib/PainPoints.svelte";
  import Roadmap from "./lib/Roadmap.svelte";
  import Intro from "./lib/Intro.svelte";
</script>

<Header />

<main>
  <Intro />
  <PainPoints />
  <Roadmap />
  <Deliverables />
  <Expert />
</main>
