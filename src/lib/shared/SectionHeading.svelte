<script lang="ts">
  let { eyebrow, title, description = "" } = $props<{
    eyebrow: string;
    title: string;
    description?: string;
  }>();
</script>

<div class="max-w-2xl mb-14">
  <span class="font-mono text-xs text-emerald-400 uppercase tracking-widest">// {eyebrow}</span>
  <h2 class="mt-3 text-3xl sm:text-4xl font-black tracking-tight text-slate-50">{title}</h2>
  {#if description}<p class="mt-4 text-slate-400 text-lg leading-relaxed">{description}</p>{/if}
</div>
