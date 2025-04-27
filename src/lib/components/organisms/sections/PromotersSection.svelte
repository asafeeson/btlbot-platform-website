<script lang="ts">
	import Anchor from '$lib/components/atoms/Anchor.svelte';
	import H2HugeColored from '$lib/components/atoms/H2HugeColored.svelte';
	import Paragraph from '$lib/components/atoms/Paragraph.svelte';
	import SectionBase from '$lib/components/atoms/SectionBase.svelte';
	const infoCardData: Record<string, string>[] = [
		{
			title: 'Контроль рабочего времени',
			body: 'Промоутер отмечает начало и окончание смены прямо в чате. Никаких табелей, только точные данные.'
		},
		{
			title: 'Геолокация (чек-ин/чек-аут)',
			body: 'Система отмечает, где находится промоутер, и позволяет понять, действительно ли он на точке. Полная прозрачность для супервайзера.'
		},
		{
			title: 'Онлайн-отчётность и статистика',
			body: 'BTLbot собирает данные в реальном времени и показывает, как идёт акция. Реагируйте сразу, пока не поздно: по конверсии, фото, чекам, выдаче призов.'
		},
		{
			title: 'Оповещения и напоминания',
			body: 'Массовые рассылки: замены, важные новости, напоминания. Всё через Telegram — быстро, понятно и без пропущенных сообщений.'
		},
		{
			title: 'Обучение промоутеров',
			body: 'Промоутеры проходят обучение и тестирование в боте перед выходом на точку. Вы точно знаете, кто готов к работе — и можете повысить стандарты.'
		},
		{
			title: 'Учёт остатков',
			body: 'Сколько продукции выдано? Где осталось? BTLbot ведёт учёт сэмплов и призов прямо в чате. Промоутер просто отмечает остатки — вам не нужно проверять вручную.'
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

<SectionBase background="white">
	<Anchor anchor="promoters"></Anchor>
	<H2HugeColored>Промоутеры</H2HugeColored>
	<div>
		<Paragraph>
			BTLbot делает работу промоутеров максимально эффективной за счет снижения нагрузки с
			супервайзера и самих промоутеров. Что позволяет им сфокусироваться на продажах. Платформа
			управляет работой промоутеров, помогает супервайзеру и собирает всю необходимую статистику.
		</Paragraph>
		<Paragraph>Всё это — в Telegram - Без приложений - Без сложных установок - Без потерь информации</Paragraph>
		<Paragraph>
			Сотрудники, промоутеры, супервайзеры и клиенты — все работают через привычный интерфейс,
			который не требует обучения.
		</Paragraph>
	</div>
	<h3>Возможности платформы</h3>
	<div class="grid grid-cols-1 gap-5 md:grid-cols-3">
		{#each infoCardData as data}
			{@render infoCard(data.title, data.body)}
		{/each}
	</div>
</SectionBase>
