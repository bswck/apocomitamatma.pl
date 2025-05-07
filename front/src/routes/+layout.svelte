<script>
	import '../app.css';
	import Social from '$lib/components/Social.svelte';
	import name from '$lib/images/name.gif';
	import Link from '$lib/components/Link.svelte';
	let year = $state(new Date().getFullYear());

	let { children } = $props();
</script>

<div
	class="fixed -z-10 h-svh w-full bg-[url('$lib/images/background.png')] bg-fixed bg-center bg-repeat blur-[5px] brightness-50"
	style="background-size: 95rem"
></div>

<div class="flex h-full w-full flex-col items-center dark:text-white">
	<div
		class="
		border-b-1 backdrop-sepia-100 border-b-(--color-outline) flex w-full
		shrink-0 grow-0 flex-col items-center justify-center gap-10
		px-6 py-2
		"
	>
		<div class="flex w-full max-w-4xl flex-col items-center sm:flex-row sm:justify-between">
			<a href="/"><img src={name} alt="apocomitamatma.pl" width="300" /></a>

			<nav aria-roledescription="Links to socials" class="flex items-center justify-center gap-5">
				<Social platform="youtube" class="text-xl" />
				<Social platform="discord" class="text-xl" />
				<Social platform="tiktok" class="text-xl" />
				<Social platform="facebook" class="text-xl" />
			</nav>
		</div>
	</div>

	<div class="shrink-1 w-full max-w-4xl flex-1">
		{@render children()}
	</div>

	<footer
		class="
		border-t-1 backdrop-sepia-100 border-t-(--color-outline)
		flex w-full shrink-0 grow-0 items-center justify-center gap-2 px-6
		py-4
		"
	>
		<div class="flex w-full max-w-4xl flex-row justify-between gap-3">
			<div class="flex flex-wrap gap-x-3 text-start">
				<Link url="/contact">Kontakt</Link>
				<Link url="/hire">Korepetycje</Link>
				<Link url="/collab">Współpraca</Link>
				<Link url="/faq">FAQ</Link>
			</div>
			<span class="hyphens-auto text-end">© {year} apocomitamatma.pl</span>
		</div>
	</footer>
</div>
