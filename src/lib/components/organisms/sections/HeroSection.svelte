<script lang="ts">
	import SectionBase from '../SectionBase.svelte';
</script>

<SectionBase background="bg-gradient-to-r from-blue-500 via-purple-500 to-pink-500">
	<div class="flex max-w-xl flex-col gap-10 py-10 mt-14 text-white">
		<h1 class="text-6xl font-black">Готовый чат-бот для BTL и промо акций</h1>
		<p>
			Всё под контролем: BTLbot автоматизирует промо-акции, работу промоутеров и коммуникацию с
			клиентами
		</p>
		<a href="http://" class="border-2 border-white px-5 py-4 hover:bg-amber-500 hover:text-black transition-colors"
			>Записаться на демо</a
		>
	</div>
	<div class="flex items-end justify-center mt-14">
		<img
			src="/robot.png"
			alt="Робот держит в руках фискальный чек Казахстан Алматы Астана"
			width="500px"
		/>
	</div>
</SectionBase>
