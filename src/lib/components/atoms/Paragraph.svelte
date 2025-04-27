<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children, extraClass }: { children: Snippet, extraClass?: string } = $props();
</script>

<p class="w-fit text-xl {extraClass}">
	{@render children()}
</p>
