<script>
  import Deliverables from "./lib/sections/Deliverables/Deliverables.svelte";
  import Expert from "./lib/sections/Expert/Expert.svelte";
  import Header from "./lib/layout/Header.svelte";
  import Intro from "./lib/sections/Intro/Intro.svelte";
  import PainPoints from "./lib/sections/PainPoints/PainPoints.svelte";
  import Roadmap from "./lib/sections/Roadmap/Roadmap.svelte";
</script>

<Header />

<main>
  <Intro />
  <PainPoints />
  <Roadmap />
  <Deliverables />
  <Expert />
</main>
