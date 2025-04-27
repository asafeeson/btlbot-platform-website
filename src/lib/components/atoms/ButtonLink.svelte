<script lang="ts">
	import type { Snippet } from 'svelte';

	let { url = '/', children }: { url: string; children: Snippet } = $props();
</script>

<a
	href={url}
	class="rounded-xl border-2 border-white px-5 py-4 transition-all hover:bg-amber-500 hover:text-black hover:shadow-2xl w-fit"
>
	{@render children()}
</a>
