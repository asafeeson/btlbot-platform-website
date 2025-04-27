<script lang="ts">
	import type { Snippet } from 'svelte';

	let { url = '/', children }: { url: string; children: Snippet } = $props();
	
</script>

<a
	href={url}
	class="border-2 border-white px-5 py-4 transition-colors hover:bg-amber-500 hover:text-black"
>
	{@render children()}
</a>
