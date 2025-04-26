<script lang="ts">
	interface MenuItem {
		url: string;
		name: string;
	}
	const menuList: MenuItem[] = [
		{ name: 'ИИ Агенты', url: '/' },
		{ name: 'BTL акции', url: '/' },
		{ name: 'Промоутеры', url: '/' },
		{ name: 'Тайный посетитель', url: '/' },
		{ name: 'Лояльность', url: '/' },
	];
</script>

<header
	class="fixed flex w-full items-end justify-between px-8 py-4 backdrop-blur backdrop-contrast-100 backdrop-saturate-100 backdrop-filter"
>
	<a href="/"><img src="/logo/colored.svg" alt="BTL бот логотип" width="80px" /></a>
	<nav class="flex gap-4">
		{#each menuList as item}
			<a href={item.url} class="transition-normal hover:font-bold">{item.name}</a>
		{/each}
	</nav>
</header>
