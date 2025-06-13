<script>
	import '../app.css';
	import Social from '$lib/components/Social.svelte';
	import name from '$lib/images/name.gif';
	let year = $state(new Date().getFullYear());

	let { children } = $props();
</script>

<!-- <div
	class="translate-z-0 absolute -z-10 h-svh w-full bg-[url('$lib/images/background.png')] bg-center bg-repeat blur-[5px] will-change-transform"
	style="background-size: 50rem"
></div> -->

<div class="flex h-full w-full flex-col items-center dark:text-white">
	{@render children()}

	<footer
		class="
		border-t-1 backdrop-sepia-100 border-t-(--color-outline)
		flex w-full shrink-0 grow-0 items-center justify-center gap-2 px-6
		py-4
		pb-5
		"
	>
		<div class="flex w-full max-w-7xl flex-col items-center sm:flex-row sm:justify-between">
			<a href="/"><img src={name} alt="apocomitamatma.pl" width="235" /></a>

			<nav aria-roledescription="Links to socials" class="flex items-center justify-center gap-5">
				<Social platform="youtube" class="text-xl" />
				<Social platform="discord" class="text-xl" />
				<Social platform="tiktok" class="text-xl" />
				<Social platform="facebook" class="text-xl" />
			</nav>
		</div>
	</footer>
</div>
