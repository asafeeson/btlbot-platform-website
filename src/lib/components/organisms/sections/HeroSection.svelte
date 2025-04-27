<script lang="ts">
	import ButtonLink from '$lib/components/atoms/ButtonLink.svelte';
	import SectionBase from '$lib/components/atoms/SectionBase.svelte';
</script>

<SectionBase background="bg-gradient-to-r from-blue-500 via-purple-500 to-pink-500 pt-30">
	<div class="flex max-w-xl flex-col gap-10 py-10 text-white">
		<h1 class="text-6xl font-black">Готовый чат-бот для BTL и промо акций</h1>
		<p>
			Всё под контролем: BTLbot автоматизирует промо-акции, работу промоутеров и коммуникацию с
			клиентами
		</p>
		<ButtonLink url="/">Записаться на демо</ButtonLink>
	</div>
	<div class="flex items-end justify-center">
		<img
			src="/robot.png"
			alt="Робот держит в руках фискальный чек Казахстан Алматы Астана"
			width="500px"
		/>
	</div>
</SectionBase>
