<script>
	import Container from '$lib/components/Container.svelte';
	import Section from '$lib/components/Section.svelte';
	import VerticalStripes from '$lib/components/VerticalStripes.svelte';

	import E8 from '$lib/images/groups/static/E8.png';
	import MP from '$lib/images/groups/static/MP.png';
	import MR from '$lib/images/groups/static/MR.png';

	import stats from '$lib/statistics.json';

	const groups = [
		{ label: 'Egzamin ósmoklasisty', key: 'E8', image: E8 },
		{ label: 'Matura podstawowa', key: 'MP', image: MP },
		{ label: 'Matura rozszerzona', key: 'MR', image: MR }
	];

	function formatCount(count) {
		const rounded = Math.round(count / 10) * 10;
		return rounded.toString() + (count % 10 === 0 ? '' : '+');
	}
</script>

<Section id="story2" class="backdrop-brightness-20">
	<VerticalStripes />
	<Container class="gap-8 py-10">
		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<h2 class="text-4xl font-bold">
				<span class="text-(--color-red)">Setki filmów,</span>
				<span class="bg-(--color-red)">tysiące</span> sukcesów
			</h2>

			<div class="grid w-full grid-cols-1 sm:grid-cols-3">
				{#each groups as { label, key, image }}
					<div
						class="border-(--color-outline) flex flex-col items-center gap-4 rounded-2xl p-6 text-center backdrop-blur-sm"
					>
						<img src={image} alt={label} class="h-32 w-auto" />
						<h3 class="text-xl font-bold">{label}</h3>
						<p class="text-2xl font-extrabold">
							<span class="bg-(--color-red)">{formatCount(stats.videoCount[key] ?? 0)}</span> filmów
						</p>
					</div>
				{/each}
			</div>
		</article>
	</Container>
</Section>
