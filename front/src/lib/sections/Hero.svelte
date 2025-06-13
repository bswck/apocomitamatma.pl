<script>
	import hire from '$lib/images/hire.png';
	import collab from '$lib/images/collab.png';
	import Sprite from '$lib/components/Sprite.svelte';
	import Social from '$lib/components/Social.svelte';
</script>

<div class="font-display backdrop-brightness-70 relative flex w-full grow-0">
	<video
		class="brightness-80 absolute -z-10 h-full w-full object-cover blur-sm"
		muted
		autoplay
		loop
		playsinline
		disablepictureinpicture
	>
		<source src="/hero.mp4" type="video/webm" />
		<source src="/hero.webm" type="video/mp4" />
	</video>

	<div
		class="pt-15 min-h-170 flex h-full w-full flex-col items-center justify-center xl:flex-row dark:text-white"
	>
		<div class="flex flex-col gap-8 text-center">
			<h1
				class="!print:text-black relative text-balance bg-white bg-clip-text text-5xl font-extrabold text-transparent"
			>
				<span class="bg-gradient from-(--color-yellow) bg-gradient-to-r to-white bg-clip-text"
					>Kolorowa</span
				>
				matematyka<br />z
				<span class="bg-gradient to-(--color-blue) bg-gradient-to-r from-white bg-clip-text"
					>humorem</span
				>
			</h1>
			<nav aria-roledescription="Links to socials" class="flex items-center justify-center gap-5">
				<Social platform="youtube" class="text-2xl" />
				<Social platform="discord" class="text-2xl" />
				<Social platform="tiktok" class="text-2xl" />
				<Social platform="facebook" class="text-2xl" />
			</nav>

			<div class="flex w-full flex-col items-center justify-evenly gap-2 p-4 lg:flex-row lg:gap-0">
				<a href="#hire" class="text-2xl font-bold">
					<div class="flex items-center gap-2 transition-all duration-300 hover:scale-125">
						<img src={hire} alt="apocomitamatma.pl" class="h-[1.5em]" />
						<span>Korepetycje</span>
					</div>
				</a>
				<a href="#collab" class="text-2xl font-bold">
					<div class="flex items-center gap-2 transition-all duration-300 hover:scale-125">
						<img src={collab} alt="apocomitamatma.pl" class="h-[1.5em]" />
						<span>Współpraca</span>
					</div>
				</a>
			</div>
		</div>

		<!-- brand.gif -->
		<Sprite class="max-h-160 static h-full min-h-80 object-cover" which="delta" />
	</div>
</div>
