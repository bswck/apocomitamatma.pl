<script>
	import Container from '$lib/components/Container.svelte';
	import Section from '$lib/components/Section.svelte';
	import VerticalStripes from '$lib/components/VerticalStripes.svelte';
</script>

<Section id="hire" class="backdrop-brightness-30 backdrop-hue-rotate-180">
	<VerticalStripes />
	<Container class="gap-8 py-10">
		<article class="w-full flex-col justify-center gap-8 text-center">
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
