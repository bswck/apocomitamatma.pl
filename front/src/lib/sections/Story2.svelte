<script>
	import Container from '$lib/components/Container.svelte';
	import Section from '$lib/components/Section.svelte';
	import VerticalStripes from '$lib/components/VerticalStripes.svelte';
</script>

<Section id="story1" class="backdrop-contrast-100">
	<VerticalStripes />
	<Container class="py-10">
		<article class="flex w-full flex-col items-center justify-center gap-8 text-center">
			<h2 class="text-4xl font-bold">
				<span class="text-(--color-red)">Ponad 750 filmów,</span> setki godzin nauki
			</h2>
			<p>
				Ogarniamy razem podstawówkę, maturę i matmę rozszerzoną. Z humorem, konkretem i <b
					>w Twoim tempie.</b
				>
			</p>
		</article>
	</Container>
</Section>
