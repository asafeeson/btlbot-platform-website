<script lang="ts">
	import type { Snippet } from 'svelte';
	let {
        color,
		size = 'text-2xl',
        font = 'font-bold', 
		children
	}: { size?: string, font?: string, color?: string; children: Snippet } = $props();
</script>

<h3 class="{font} {size} {color}">{@render children()}</h3>
