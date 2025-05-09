<script>
	import hire from '$lib/images/hire.gif';
	import collab from '$lib/images/collab.png';
	import Sprite from '$lib/components/Sprite.svelte';
</script>

<div class="relative w-full grow">
	<div
		class="pt-15 flex h-full w-full flex-col items-center justify-center xl:flex-row dark:text-white"
	>
		<div class="flex flex-col gap-4 text-center">
			<h1
				class="!print:text-black relative text-balance bg-white bg-clip-text text-5xl font-extrabold text-transparent"
			>
				<span class="bg-gradient from-(--color-yellow) bg-gradient-to-r to-white bg-clip-text"
					>Kolorowa</span
				>
				matematyka<br />z poczuciem
				<span class="bg-gradient to-(--color-blue) bg-gradient-to-r from-white bg-clip-text"
					>humoru</span
				>
			</h1>

			<div class="flex w-full flex-col items-center justify-evenly gap-2 p-4 lg:flex-row lg:gap-0">
				<a href="#hire" class="text-2xl font-bold">
					<div class="flex items-center gap-2 transition-all duration-300 hover:scale-125">
						<img src={hire} alt="apocomitamatma.pl" class="h-[1.5em]" />
						<span>Matma</span>
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
		<Sprite class="max-h-160 static h-full min-h-80 object-cover" which="delta" />
	</div>
</div>
