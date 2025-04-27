<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children, background }: { children: Snippet; background?: string } = $props();
</script>

<section
	class="min-h-xl flex flex-wrap items-start justify-between gap-10 {background} p-14 lg:px-20"
>
	<div
		class="rounded-4xl border border-gray-200 px-10 py-14 shadow-lg transition-shadow hover:shadow-2xl"
	>
		{@render children()}
	</div>
</section>
