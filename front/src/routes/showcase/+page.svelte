<script>
	import NowaEra from '$lib/images/partners/nowaera.png';
	import PWN from '$lib/images/partners/pwn.png';
	import SWPS from '$lib/images/partners/swps.png';
	import WSKZ from '$lib/images/partners/wskz.png';
	import Link from '$lib/components/Link.svelte';
</script>

<div class="mx-auto flex h-min w-full grow flex-col items-center">
	<div class="mx-auto flex w-full max-w-7xl flex-col items-center gap-8 p-8">
		<h1 class="text-3xl font-bold">Przykłady lokowania</h1>

		<div class="flex w-full flex-col gap-8">
			<div class="flex items-center justify-center gap-8">
				<Link newTab={true} url="https://www.nowaera.pl/">
					<img src={NowaEra} alt="Nowa Era" class="h-auto w-60 object-cover" /></Link
				>

				<iframe
					class="aspect-video w-full"
					src="https://www.youtube-nocookie.com/embed/Mi710Z_K5Y8"
					title=""
					frameborder="0"
					allow="clipboard-write; encrypted-media; picture-in-picture;"
					allowfullscreen
				></iframe>
			</div>
			<div class="flex items-center justify-center gap-8">
				<Link newTab={true} url="https://www.pwn.pl/">
					<img src={PWN} alt="PWN" class="h-auto w-60 object-contain" />
				</Link>

				<iframe
					class="aspect-video w-full"
					src="https://www.youtube-nocookie.com/embed/MXeGVBp5PCw"
					title=""
					frameborder="0"
					allow="clipboard-write; encrypted-media; picture-in-picture;"
					allowfullscreen
				></iframe>
			</div>
			<div class="flex items-center justify-center gap-8">
				<Link newTab={true} url="https://www.swps.pl/">
					<img src={SWPS} alt="SWPS" class="h-auto w-60 object-contain" />
				</Link>

				<iframe
					class="aspect-video w-full"
					src="https://www.youtube-nocookie.com/embed/EXOUgyFomxs"
					title=""
					frameborder="0"
					allow="clipboard-write; encrypted-media; picture-in-picture;"
					allowfullscreen
				></iframe>
			</div>

			<div class="flex items-center justify-center gap-8">
				<Link newTab={true} url="https://www.wskz.pl/">
					<img src={WSKZ} alt="WSKZ" class="h-auto w-60 object-cover" /></Link
				>

				<iframe
					class="aspect-video w-full"
					src="https://www.youtube-nocookie.com/embed/rM9VeXkSVpw"
					title=""
					frameborder="0"
					allow="clipboard-write; encrypted-media; picture-in-picture;"
					allowfullscreen
				></iframe>
			</div>
		</div>
	</div>
</div>
