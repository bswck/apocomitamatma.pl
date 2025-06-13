<script>
	import Container from '$lib/components/Container.svelte';
	import FormulaBubbles from '$lib/components/FormulaBubbles.svelte';
	import Section from '$lib/components/Section.svelte';
	import Sprite from '$lib/components/Sprite.svelte';
	import CTAButton from '$lib/components/CTAButton.svelte';
</script>

<Section id="hire-details" class="grow-0 backdrop-blur-[3.5px]">
	<Container class="gap-8 py-10 xl:pb-0 xl:pt-10">
		<Sprite class="max-h-120 block h-full	min-h-60 object-cover" which="figures" />
		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<h2 class="text-4xl font-bold">
				Za rączkę <span class="text-(--color-yellow)">do celu</span>
			</h2>
			<CTAButton
				text="Zgłoś się na korki"
				color="red"
				email="kontakt@apocomitamatma.pl"
				phoneNumber="+48 665 165 432"
			/>
		</article>
	</Container>
</Section>
