<script lang="ts">
	const menuList = ['ИИ Агенты', 'BTL акции', 'Промоутеры', 'Тайный посетитель', 'Лояльность'];
</script>

<section class="py-8">
	<nav class="flex flex-wrap justify-center gap-5">
		{#each menuList as item}
			<a href="/" class="px-5 py-2 bg-blue-600 rounded-3xl text-white hover:bg-blue-500 transition-colors">{item}</a>
		{/each}
	</nav>
</section>
