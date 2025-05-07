<script>
	import Sprite from '$lib/components/Sprite.svelte';
	import brand from '$lib/images/brand.gif';
</script>

<div
	role="presentation"
	class="lg:min-h-50 mx-auto flex h-min flex-col items-center justify-center gap-4"
>
	<article class="max-w-2/3 text-center">
		<img class="mx-auto aspect-auto h-20 object-contain" src={brand} alt="apocomitamatma.pl" />
		<h1 class="text-balance text-2xl">Kolorowa matematyka z poczuciem humoru.</h1>
		<p class="text-xl"></p>
	</article>
	<Sprite
		class="max-h-180 min-h-120 absolute bottom-0 hidden h-full object-cover lg:block"
		which="delta"
	/>
</div>
