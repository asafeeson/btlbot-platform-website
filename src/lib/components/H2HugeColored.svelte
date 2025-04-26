<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children }: { children: Snippet } = $props();
</script>

<h2
	class="w-fit bg-gradient-to-tl from-slate-800 via-violet-500 to-zinc-400 bg-clip-text text-9xl/[0.9] font-black text-transparent"
>
	{@render children()}
</h2>
