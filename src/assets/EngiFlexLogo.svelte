<script lang="ts">
  import type { SVGAttributes } from "svelte/elements";

  let { class: className = "", ...rest }: SVGAttributes<SVGSVGElement> =
    $props();
</script>

<svg
  class={className}
  viewBox="0 0 214 48"
  fill="none"
  xmlns="http://www.w3.org/2000/svg"
  role="img"
  aria-label="EngiFlex — Flexible in Engineering"
  {...rest}
>
  <defs>
    <linearGradient
      id="engiflex-grad"
      x1="8"
      y1="8"
      x2="40"
      y2="40"
      gradientUnits="userSpaceOnUse"
    >
      <stop offset="0" stop-color="#A855F7"></stop>
      <stop offset="0.5" stop-color="#3B82F6"></stop>
      <stop offset="1" stop-color="#10B981"></stop>
    </linearGradient>
  </defs>
  <path
    d="M8,14 L8,34 Q8,40 13.36,37.32 L34.64,26.68 Q40,24 34.64,21.32 L13.36,10.68 Q8,8 8,14 Z"
    fill="url(#engiflex-grad)"
  ></path>
  <path
    d="M10.77,15.16 L10.77,32.84 Q10.77,35.84 13.47,34.52 L32.31,25.32 Q35.01,24 32.31,22.68 L13.47,13.48 Q10.77,12.16 10.77,15.16 Z"
    fill="#0F172A"
  ></path>
  <text
    x="50"
    y="27"
    fill="#FFFFFF"
    font-family="Inter, ui-sans-serif, system-ui, sans-serif"
    font-size="20"
    font-weight="800"
    letter-spacing="-0.5">EngiFlex</text
  >
  <text
    x="50"
    y="40"
    fill="#FFFFFF"
    font-family="Inter, ui-sans-serif, system-ui, sans-serif"
    font-size="6.5"
    font-weight="600"
    letter-spacing="2">FLEXIBLE IN ENGINEERING</text
  >
</svg>
