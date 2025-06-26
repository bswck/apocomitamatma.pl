<script>
	import hire from '$lib/images/hire.png';
	import collab from '$lib/images/collab.png';
	import Sprite from '$lib/components/Sprite.svelte';
	import Social from '$lib/components/Social.svelte';
	import ytImg from '$lib/images/icons/yt.png';
	import dcImg from '$lib/images/icons/dc.png';
	import Link from '$lib/components/Link.svelte';
</script>

<div class="font-display backdrop-brightness-70 relative flex w-full grow-0">
	<video
		class="brightness-60 absolute -z-10 h-full w-full object-cover blur-sm"
		muted
		autoplay
		loop
		playsinline
		disablepictureinpicture
	>
		<source src="/hero.mp4" type="video/mp4" />
		<source src="/hero.webm" type="video/webm" />
	</video>

	<div
		class="pt-15 min-h-170 flex h-full w-full flex-col items-center justify-center xl:flex-row dark:text-white"
	>
		<div class="flex flex-col items-center gap-8 text-center">
			<h1
				class="!print:text-black relative text-balance bg-white bg-clip-text text-5xl font-extrabold text-transparent"
			>
				Kolorowa matematyka<br />z humorem
			</h1>
			<nav aria-roledescription="Links to socials" class="flex w-1/2 items-center justify-evenly">
				<Social platform="youtube"><img class="w-16" src={ytImg} alt="" /></Social>
				<Social platform="discord"><img class="w-16" src={dcImg} alt="" /></Social>
			</nav>

			<div class="flex w-full flex-col items-center justify-evenly gap-4 p-4 lg:flex-row lg:gap-0">
				<Link
					url="#hire"
					class="border-(--color-outline) border-3 flex items-center gap-2 rounded-2xl p-2 text-2xl font-bold"
				>
					<img src={hire} alt="apocomitamatma.pl" class="h-[1.5em]" />
					<span>Korepetycje</span>
				</Link>
				<Link
					url="#collab"
					class="border-(--color-outline) border-3 flex items-center gap-2 rounded-2xl p-2 text-2xl font-bold"
				>
					<img src={collab} alt="apocomitamatma.pl" class="h-[1.5em]" />
					<span>Współpraca</span>
				</Link>
			</div>
		</div>

		<!-- brand.gif -->
		<Sprite class="max-h-160 static h-full lg:object-cover" which="delta" />
	</div>
</div>
