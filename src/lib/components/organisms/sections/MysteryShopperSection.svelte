<script lang="ts">
	import Anchor from '$lib/components/atoms/Anchor.svelte';
	import H2HugeColored from '$lib/components/atoms/H2HugeColored.svelte';
	import Paragraph from '$lib/components/atoms/Paragraph.svelte';
	import SectionBase from '$lib/components/atoms/SectionBase.svelte';

	interface infoCard {
		title: string;
		body: string;
	}
	const infoCardData: infoCard[] = [
		{
			title: '🕒 Контроль визита тайного покупателя',
			body: 'Тайный покупатель фиксирует начало и окончание визита через AI чат-бот. Больше никаких бумажных анкет и Excel-файлов — только чёткие данные в реальном времени.'
		},
		{
			title: '📍 Геолокация (чек-ин/чек-аут)',
			body: 'Система отмечает, где именно был сделан визит. Нейросети для бизнеса проверяют соответствие маршрута заданным точкам, исключая подделку результатов. Искусственный интеллект в маркетинге помогает получать честные данные.'
		},
		{
			title: '📊 Онлайн-отчётность и аналитика',
			body: 'BTLbot собирает все данные в момент посещения: ответы на вопросы, фото витрины, подтверждение покупки. Отчёт по каждому визиту строится автоматически. Примеры ИИ в бизнесе показывают, что правильная аналитика = точные управленческие решения.'
		},
		{
			title: '📣 Оповещения и корректировки',
			body: 'Если правила проверки меняются, бот моментально уведомляет всех тайных покупателей. Через Telegram они получают инструкции, замены точек или напоминания. Чат-боты для CRM обеспечивают полную координацию без дополнительных звонков и писем.'
		},
		{
			title: '🧠 Обучение тайных покупателей',
			body: 'Перед началом проекта тайные покупатели проходят обучение через ИИ помощник для консультаций. Это позволяет повысить качество проверок и минимизировать ошибки.'
		},
		{
			title: '📦 Фиксация результатов проверок',
			body: 'Каждая анкета, чек, фото — отправляются сразу в систему через чат. Автоматизация клиентского сервиса позволяет в реальном времени видеть качество обслуживания и вовремя реагировать.'
		}
	];
</script>

{#snippet infoCard(title: string, body: string)}
	<div
		class="rounded-xl border border-gray-200 p-5 transition-all hover:border-purple-500 hover:shadow-lg"
	>
		<h4 class="mb-1.5 text-xl font-bold">{title}</h4>
		<p>{body}</p>
	</div>
{/snippet}

<SectionBase background="">
	<Anchor anchor="mystery-shopper"></Anchor>
	<H2HugeColored>Тайный Покупатель</H2HugeColored>
	<span class="-mt-5 bg-pink-500 px-3 py-1 text-2xl text-white"
		>Чат-бот для акций экономит до 70% времени на сбор и обработку данных</span
	>

	<Paragraph>
		Платформа позволяет создать задание, выслать его тайному посетителю, собрать фото, чек и фидбэк
		— всё через чат. Сразу же доступны отчёты и статистика. Больше никаких бумажных анкет и
		Excel-файлов — только чёткие данные в реальном времени.
	</Paragraph>
	<div class="grid grid-cols-1 gap-5 md:grid-cols-3">
		{#each infoCardData as data}
			{@render infoCard(data.title, data.body)}
		{/each}
	</div>
</SectionBase>
