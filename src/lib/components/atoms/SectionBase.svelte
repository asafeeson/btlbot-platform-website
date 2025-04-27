<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children, background }: { children: Snippet, background?: string } = $props();
</script>

<section class="flex flex-wrap items-start min-h-xl justify-between gap-10 {background} p-14 lg:px-20">
    {@render children()}
</section>

