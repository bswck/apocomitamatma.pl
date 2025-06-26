<script>
	import Section from '$lib/components/Section.svelte';
	import CTAButton from '$lib/components/CTAButton.svelte';

	import E8 from '$lib/images/groups/static/E8.png';
	import MP from '$lib/images/groups/static/MP.png';
	import MR from '$lib/images/groups/static/MR.png';

	import stats from '$lib/statistics.json';

	const groups = [
		{ label: 'Egzamin ósmoklasisty', key: 'E8', image: E8 },
		{ label: 'Matura podstawowa', key: 'MP', image: MP },
		{ label: 'Matura rozszerzona', key: 'MR', image: MR }
	];

	/**
	 * @param {number} count
	 */
	function formatCount(count) {
		const rounded = Math.round(count / 10) * 10;
		return rounded.toString() + (count % 10 === 0 ? '' : '+');
	}
</script>

<Section id="hire" class="backdrop-brightness-30 backdrop-hue-rotate-180">
	<div
		class="brightness-30 absolute -z-10 h-full w-full bg-[url('$lib/images/background.png')] bg-center bg-repeat blur-[2.5px]"
		style="background-size: 100rem"
	></div>
	<div class="flex flex-col gap-8 py-10">
		<article class="w-full flex-col justify-center gap-8 text-center">
			<h2 class="text-4xl font-bold">
				<span class="bg-(--color-red)">Zacznij</span> rozumieć matematykę
			</h2>
		</article>

		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<div class="grid w-full grid-cols-1 sm:grid-cols-3">
				{#each groups as { label, key, image }}
					<div
						class="border-(--color-outline) flex flex-col items-center gap-4 rounded-2xl p-6 text-center"
					>
						<img src={image} alt={label} class="h-32 w-auto" />
						<h3 class="text-xl font-bold">{label}</h3>
						<p class="text-2xl font-extrabold">
							<span class="bg-(--color-red)">{formatCount(stats.videoCount[key])}</span> filmów
						</p>
					</div>
				{/each}
			</div>
		</article>
		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<CTAButton
				text="Umów zajęcia"
				color="red"
				email="kontakt@apocomitamatma.pl"
				phoneNumber="+48 665 165 432"
			/>
		</article>
	</div>
</Section>
