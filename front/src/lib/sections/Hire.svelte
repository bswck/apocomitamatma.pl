<script>
	import Container from '$lib/components/Container.svelte';
	import FormulaBubbles from '$lib/components/FormulaBubbles.svelte';
	import Section from '$lib/components/Section.svelte';
	import Sprite from '$lib/components/Sprite.svelte';
</script>

<Section id="hire" class="backdrop-contrast-125">
	<FormulaBubbles />
	<Container class="pt-10">
		<Sprite class="max-h-160 block h-full min-h-80 object-cover" which="figures" />
		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<h2 class="text-4xl font-bold">
				Za rączkę <span class="text-(--color-yellow)">do celu</span>
			</h2>
			<p>
				Szukasz kogoś, kto pokaże Ci, że matma ma sens? U mnie nie ma głupich pytań. Tłumaczę z
				luzem, ale bez ściemy.
			</p>
			<p>
				Przygotuję Cię do matury (podstawa i rozszerzenie), egzaminu ósmoklasisty lub poprawy ocen.
				Wszystko z jasnym planem i pełnym wsparciem.
			</p>
		</article>
	</Container>
</Section>
