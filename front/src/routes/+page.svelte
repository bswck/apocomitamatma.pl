<script>
	import Collab from '$lib/sections/Collab.svelte';
	import Hero from '$lib/sections/Hero.svelte';
	import Hire from '$lib/sections/Hire.svelte';
	import Story1 from '$lib/sections/Story1.svelte';
	import Story2 from '$lib/sections/Story2.svelte';
</script>

<div class="mx-auto flex h-min w-full grow flex-col items-center">
	<Hero />
	<Story1 />
	<Hire />
	<Story2 />
	<Collab />
</div>
