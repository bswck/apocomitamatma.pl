<script>
	import Collab from '$lib/sections/Collab.svelte';
	import Hero from '$lib/sections/Hero.svelte';
	import Hire from '$lib/sections/Hire.svelte';
	import HireDetails from '$lib/sections/HireDetails.svelte';
	import Story2 from '$lib/sections/Story2.svelte';
</script>

<div class="mx-auto flex h-min w-full grow flex-col items-center">
	<Hero />
	<div class="relative w-full">
		<div
			class="absolute h-full w-full bg-[url('$lib/images/background.png')] bg-center bg-repeat blur-[1px] brightness-50"
			style="background-size: 30rem"
		></div>

		<Hire />
		<HireDetails />
		<Story2 />
	</div>
	<Collab />
</div>
