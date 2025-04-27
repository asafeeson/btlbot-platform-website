<script lang="ts">
	import SectionBase from '$lib/components/atoms/SectionBase.svelte';
	import H2HugeColored from '$lib/components/atoms/H2HugeColored.svelte';
	import Paragraph from '$lib/components/atoms/Paragraph.svelte';
</script>

<SectionBase background="bg-amber-50">
	<div class="flex flex-wrap items-center justify-between gap-20 lg:flex-nowrap">
		<H2HugeColored>больше чем просто чат-бот</H2HugeColored>
		<Paragraph>
			BTLbot — это AI-платформа нового поколения, которая управляет всей BTL-механикой ваших акций.
			От работы промоутеров до розыгрышей, обучения и лояльности — всё, что раньше требовало
			десятков Excel-файлов и координации по телефону, WhatsApp чатах, теперь решается автоматически
			и без ошибок.
		</Paragraph>
	</div>
</SectionBase>
