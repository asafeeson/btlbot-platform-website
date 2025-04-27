<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children, background, innerExtraClass }: { children: Snippet; background?: string, innerExtraClass?: string } = $props();
</script>

<section
	class="min-h-xl {background} p-14 lg:px-20"
>
	<div
		class="flex flex-wrap items-start justify-between gap-10 rounded-4xl border border-gray-200 px-10 py-14 shadow-lg transition-shadow hover:shadow-2xl {innerExtraClass}"
	>
		{@render children()}
	</div>
</section>
