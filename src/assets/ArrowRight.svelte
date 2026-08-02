<script lang="ts">
  import type { SVGAttributes } from "svelte/elements";

  let { class: className = "", ...rest }: SVGAttributes<SVGSVGElement> =
    $props();
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  width="24"
  height="24"
  viewBox="0 0 24 24"
  fill="none"
  stroke="currentColor"
  stroke-width="2"
  stroke-linecap="round"
  stroke-linejoin="round"
  class={className}
  aria-hidden="true"
  {...rest}
>
  <path d="M5 12h14"></path>
  <path d="m12 5 7 7-7 7"></path>
</svg>
