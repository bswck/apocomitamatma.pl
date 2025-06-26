<script>
	import Section from '$lib/components/Section.svelte';
	import CTAButton from '$lib/components/CTAButton.svelte';

	import Container from '$lib/components/Container.svelte';
	import Cards from './Cards.svelte';
</script>

<Section id="hire" class="backdrop-brightness-30 backdrop-hue-rotate-180">
	<div
		class="brightness-20 absolute -z-10 h-full w-full bg-[url('$lib/images/background.png')] bg-center bg-repeat blur-[2.5px]"
		style="background-size: 85rem"
	></div>
	<div class="flex flex-col items-center gap-10 py-10 text-center">
		<h2 class="text-4xl font-bold">Zacznij rozumieć matematykę</h2>

		<Cards />
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
