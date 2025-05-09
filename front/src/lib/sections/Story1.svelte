<script>
	import Container from '$lib/components/Container.svelte';
	import Section from '$lib/components/Section.svelte';
	import VerticalStripes from '$lib/components/VerticalStripes.svelte';
</script>

<Section id="story1" class="backdrop-hue-rotate-180">
	<VerticalStripes />
	<Container class="py-10">
		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<h2 class="text-4xl font-bold">
				<span class="text-(--color-blue)">Nowy standard</span> w nauce matmy
			</h2>
			<p>
				Zaczęło się od kilku filmów w pandemii, dziś to jedno z najważniejszych miejsc w polskim
				YouTube edukacyjnym. Matematyka – bez stresu, bez nudy, ale zawsze na serio.
			</p>
		</article>
	</Container>
</Section>
