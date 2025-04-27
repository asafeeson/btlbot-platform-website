<script lang="ts">
	import H2HugeColored from '$lib/components/atoms/H2HugeColored.svelte';
	import Paragraph from '$lib/components/atoms/Paragraph.svelte';
	import SectionBase from '$lib/components/atoms/SectionBase.svelte';

	const infoCardData = [{ title: 'AI для бизнеса', body: '' }];
</script>

{#snippet infoCard(title: string, body: string)}
	<div
		class="rounded-xl border border-gray-200 p-5 transition-all hover:border-purple-500 hover:shadow-lg"
	>
		<h4 class="mb-1.5 text-xl font-bold">{title}</h4>
		<p>{body}</p>
	</div>
{/snippet}

{#snippet attractiveBullets(number: string, title: string, color: string)}
	<div class="flex items-center gap-3">
		<span
			class="flex min-h-10 min-w-10 items-center justify-center rounded bg-{color}-500 font-medium text-white"
		>
			{number}
		</span>
		<p class="w-fit font-medium">{title}</p>
	</div>
{/snippet}

<SectionBase innerExtraClass="flex-col">
	<H2HugeColored>AI-агенты</H2HugeColored>
	<span class="-mt-5 bg-pink-500 px-3 py-1 text-2xl text-white"
		>Ваш новый герой промо-акций и сотрудник без выходных !</span
	>
	<div class="flex gap-10">
		<div
			class="basis-1/3 space-y-5 rounded-xl border border-gray-200 p-5 transition-all hover:border-purple-500 hover:shadow-lg"
		>
			<h5 class="text-xl font-bold">Агент для бизнеса</h5>
			<p>
				AI-агент — это ваш новый инструмент для автоматизации процессов внутри компании и упрощения
				взаимодействия с клиентами. Это автоматизация, которая работает на результат!
			</p>
            <p>
				Достаточно настроить архитектуру AI-бота и подготовить технический фронт — и он начнет
				выполнять рутинные задачи за вас. Меньше ручной работы. Больше эффективности. Больше роста.
			</p>
			<p>С его помощью вы можете:</p>
            <div class="space-y-4">
				{@render attractiveBullets('1', 'Проводить автоматическое анкетирование', 'pink')}
				{@render attractiveBullets('2', 'Формировать контракты и методички для сотрудников', 'purple')}
				{@render attractiveBullets('3', 'Создавать отчёты и маркетинговые стратегии', 'blue')}
				{@render attractiveBullets('5', 'Строить SEO-ядра для сайтов', 'green')}
				{@render attractiveBullets('6', 'Организовать работу команды быстрее и проще', 'amber')}
			</div>

		</div>
		<div
			class="basis-1/3 space-y-5 rounded-xl border border-gray-200 p-5 transition-all hover:border-purple-500 hover:shadow-lg"
		>
			<h5 class="text-xl font-bold">Агент для продаж</h5>
			<p>
				Увеличьте эффективность отдела продаж с помощью AI-агента — цифрового сотрудника, который:
			</p>
			<ul>
				<li>Работает 24/7 без зарплаты и отпусков</li>
				<li>Молниеносно отвечает на запросы клиентов</li>
				<li>Всегда в хорошем настроении</li>
				<li>Использует обширную базу знаний о ваших товарах</li>
			</ul>
			<p>
				AI-агент подстраивается под заданный промпт: расскажет о наличии на складе, посоветует
				лучший вариант, объяснит особенности использования продукта и поможет подобрать нужное
				решение. А затем — передаст менеджерам контакты уже "тёплых" клиентов, готовых к переговорам
				и оплате.
			</p>
			<div class="space-y-4">
				{@render attractiveBullets('1', 'Больше продаж', 'pink')}
				{@render attractiveBullets('2', 'Меньше затрат', 'purple')}
				{@render attractiveBullets('3', 'Максимальная скорость реакции', 'blue')}
			</div>
		</div>
		<div
			class="basis-1/3 space-y-5 rounded-xl border border-gray-200 p-5 transition-all hover:border-purple-500 hover:shadow-lg"
		>
			<h5 class="text-xl font-bold">Агент для маркетинга</h5>
			<p>
				Запустите свою промо- или digital-акцию с уникальным AI-маскотом! Искусственный интеллект
				будет играть заданную роль: AI-маскот может стать лицом вашей рекламной кампании — или
				стильной ее частью, цифровым проумолтером, который вовлечёт аудиторию и сделает вашу акцию
				ярче и интереснее. Эмоции, вовлеченность и вау-эффект — без лишних затрат на персонал.
			</p>
			<div class="space-y-4">
				{@render attractiveBullets('1', 'Бариста, который помогает выбрать идеальный кофе', 'pink')}
				{@render attractiveBullets(
					'2',
					'Дерматолог, который советует косметику под ваш тип кожи',
					'purple'
				)}
				{@render attractiveBullets('3', 'Фармацевт, который подбирает витамины и БАДы', 'blue')}
				{@render attractiveBullets(
					'4',
					'Или даже творческий AI-художник, который создаёт уникальные картинки по фото участников',
					'green'
				)}
			</div>
		</div>
	</div>
</SectionBase>
