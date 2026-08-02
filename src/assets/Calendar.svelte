<script lang="ts">
  import type { SVGAttributes } from 'svelte/elements'

  let { class: className = '', ...rest }: SVGAttributes<SVGSVGElement> = $props()
</script>

<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class={className} aria-hidden="true" {...rest}>
  <path d="M8 2v4"></path>
  <path d="M16 2v4"></path>
  <rect width="18" height="18" x="3" y="4" rx="2"></rect>
  <path d="M3 10h18"></path>
</svg>
