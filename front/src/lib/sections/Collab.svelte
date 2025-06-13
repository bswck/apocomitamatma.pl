<script>
	import Container from '$lib/components/Container.svelte';
	import Section from '$lib/components/Section.svelte';
	import Sprite from '$lib/components/Sprite.svelte';
	import CTAButton from '$lib/components/CTAButton.svelte';
	import Partners from '$lib/components/Partners.svelte';
</script>

<Section id="collab" class="backdrop-brightness-50">
	<!-- <VerticalStripes id="1" size="5rem" blur="2px" /> -->
	<Container class="pt-10">
		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<h2 class="text-4xl font-bold">
				Szukasz partnera do <span class="text-(--color-blue)">edukacyjnych projektów</span>?
			</h2>
			<CTAButton text="Nawiąż współpracę" color="blue" email="wspolpraca@apocomitamatma.pl" />
		</article>

		<Sprite class="max-h-120 hidden h-full min-h-20 object-cover lg:block" which="rizz" />
		<Partners />
	</Container>
</Section>
