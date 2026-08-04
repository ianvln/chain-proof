<script>
  import Deliverables from "./lib/sections/Deliverables/Deliverables.svelte";
  import Expert from "./lib/sections/Expert/Expert.svelte";
  import Header from "./lib/layout/Header.svelte";
  import Intro from "./lib/sections/Intro/Intro.svelte";
  import Partnership from "./lib/sections/Partnership/Partnership.svelte";
  import PainPoints from "./lib/sections/PainPoints/PainPoints.svelte";
  import Roadmap from "./lib/sections/Roadmap/Roadmap.svelte";
  import Footer from "./lib/layout/Footer.svelte";
</script>

<Header />

<main>
  <Intro />
  <Partnership />
  <PainPoints />
  <Roadmap />
  <Deliverables />
  <Expert />
</main>

<Footer />
