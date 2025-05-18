<script>
	import Container from '$lib/components/Container.svelte';
	import Section from '$lib/components/Section.svelte';
	import Sprite from '$lib/components/Sprite.svelte';
	import CTAButton from '$lib/components/CTAButton.svelte';
</script>

<Section id="collab" class="backdrop-brightness-50">
	<!-- <VerticalStripes id="1" size="5rem" blur="2px" /> -->
	<Container class="pt-10">
		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<h2 class="text-4xl font-bold">
				Gramy do <span class="text-(--color-blue)">tej samej bramki</span>
			</h2>
			<p>
				Edukacja to gra zespołowa – jestem otwarty na współpracę z markami, twórcami i
				nauczycielami, którym bliska jest misja dzielenia się wiedzą.
			</p>
			<p>
				Szukasz partnera do wspólnych działań edukacyjnych? Odezwij się – chętnie podejmę
				wartościowe współprace.
			</p>
			<CTAButton
				text="Napisz i zaproponuj współpracę"
				color="blue"
				email="wspolpraca@apocomitamatma.pl"
			/>
		</article>

		<Sprite class="max-h-160 block h-full min-h-80 object-cover" which="rizz" />
	</Container>
</Section>
