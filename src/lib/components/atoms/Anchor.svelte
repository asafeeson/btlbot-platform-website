<script lang="ts">
	import type { Snippet } from 'svelte';

	let { anchor }: { anchor: string } = $props();
</script>

<div id={anchor}></div>