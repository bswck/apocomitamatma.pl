<script>
	import Card from './Card.svelte';
	import Link from '$lib/components/Link.svelte';
	import E8 from '$lib/images/groups/static/E8.png';
	import MP from '$lib/images/groups/static/MP.png';
	import MR from '$lib/images/groups/static/MR.png';
	import Container from '$lib/components/Container.svelte';
	import statistics from '$lib/statistics.json';

	/** @param {number} count */
	function formatCount(count) {
		const rounded = Math.round(count / 10) * 10;
		return rounded.toString() + (count % 10 === 0 ? '' : '+');
	}
</script>

<Container class="gap-8">
	<Card class="lg:mt-16">
		<div class="flex flex-row items-center gap-4">
			<div>
				<img src={E8} alt="Egzamin ósmoklasisty" class="h-16 w-auto" />
			</div>
			<div>
				<h3 class="text-(--color-blue) text-2xl font-semibold">Egzamin ósmoklasisty</h3>
			</div>
		</div>
		<div class="text-balance">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos autem eum nobis, modi culpa
			temporibus nulla fuga magni facere, blanditiis vero, cumque accusamus pariatur maxime
			perspiciatis dolorem.
		</div>

		<strong class="text-2xl font-extrabold">
			{formatCount(statistics.videoCount.E8)} filmów
		</strong>

		<iframe
			class="aspect-video w-full"
			src="https://www.youtube-nocookie.com/embed/videoseries?list=PL1FMwXulgdSRnqH9sxiU79UyGFXF1RWes"
			title=""
			frameborder="0"
			allow="clipboard-write; encrypted-media; picture-in-picture;"
			allowfullscreen
		></iframe>

		<div class="flex flex-row items-center justify-evenly">
			<div class="flex-3">Potrzebujesz korepetycji?</div>
			<Link url="kontakt@apocomitamatma.pl" class="flex-4 bg-(--color-blue) p-2 font-semibold"
				>Umów zajęcia</Link
			>
		</div>
	</Card>

	<Card>
		<div class="flex flex-row items-center gap-4">
			<div>
				<img src={MP} alt="Matura podstawowa" class="h-16 w-auto" />
			</div>
			<div>
				<h3 class="text-(--color-yellow) text-2xl font-semibold">Matura podstawowa</h3>
			</div>
		</div>
		<div class="text-balance">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos autem eum nobis, modi culpa
			temporibus nulla fuga magni facere, blanditiis vero, cumque accusamus pariatur maxime
			perspiciatis dolorem.
		</div>

		<strong class="text-2xl font-extrabold">
			{formatCount(statistics.videoCount.MP)} filmów
		</strong>

		<iframe
			class="aspect-video w-full"
			src="https://www.youtube-nocookie.com/embed/videoseries?list=PL1FMwXulgdSSUCJ4jbMcCeAqgSKKjQFRU"
			title=""
			frameborder="0"
			allow="clipboard-write; encrypted-media; picture-in-picture;"
			allowfullscreen
		></iframe>

		<div class="flex flex-row items-center justify-evenly">
			<div class="flex-3">Potrzebujesz korepetycji?</div>
			<Link
				url="mailto:kontakt@apocomitamatma.pl"
				class="flex-4 bg-(--color-yellow) p-2 font-semibold text-black"
			>
				Umów zajęcia
			</Link>
		</div>
	</Card>

	<Card class="lg:mt-16">
		<div class="flex flex-row items-center gap-4">
			<div>
				<img src={MR} alt="Matura rozszerzona" class="h-16 w-auto" />
			</div>
			<div>
				<h3 class="text-(--color-red) text-2xl font-semibold">Matura rozszerzona</h3>
			</div>
		</div>
		<div class="text-balance">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos autem eum nobis, modi culpa
			temporibus nulla fuga magni facere, blanditiis vero, cumque accusamus pariatur maxime
			perspiciatis dolorem.
		</div>

		<strong class="text-2xl font-extrabold">
			{formatCount(statistics.videoCount.MR)} filmów
		</strong>

		<iframe
			class="aspect-video w-full"
			src="https://www.youtube-nocookie.com/embed/videoseries?list=PL1FMwXulgdSR9D9jJZTdPWRpSutzEq2WA"
			title=""
			frameborder="0"
			allow="clipboard-write; encrypted-media; picture-in-picture;"
			allowfullscreen
		></iframe>

		<div class="flex flex-row items-center justify-evenly">
			<div class="flex-3">Potrzebujesz korepetycji?</div>
			<Link url="kontakt@apocomitamatma.pl" class="flex-4 bg-(--color-red) p-2 font-semibold"
				>Umów zajęcia
			</Link>
		</div>
	</Card>
</Container>
