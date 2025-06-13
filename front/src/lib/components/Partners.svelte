<script>
	import NowaEra from '$lib/images/partners/nowaera.png';
	import PWN from '$lib/images/partners/pwn.png';
	import SWPS from '$lib/images/partners/swps.png';
	import WSKZ from '$lib/images/partners/wskz.png';
	import Link from './Link.svelte';
</script>

<div class="flex w-full flex-col items-center justify-center gap-4 p-8">
	<h2 class="text-2xl font-bold">Partnerzy</h2>
	<div class="flex flex-col items-center justify-center gap-4">
		<div class="flex flex-row gap-4">
			<Link newTab={true} url="https://youtu.be/Mi710Z_K5Y8">
				<img src={NowaEra} alt="Nowa Era" class="h-auto w-60 object-cover" />
			</Link>
			<Link newTab={true} url="https://youtu.be/MXeGVBp5PCw">
				<img src={PWN} alt="PWN" class="h-auto w-60 object-contain" />
			</Link>
		</div>
		<div class="flex flex-col gap-4 md:flex-row">
			<Link newTab={true} url="https://youtu.be/EXOUgyFomxs">
				<img src={SWPS} alt="SWPS" class="h-auto w-60 object-contain" />
			</Link>
			<Link newTab={true} url="https://youtu.be/rM9VeXkSVpw">
				<img src={WSKZ} alt="WSKZ" class="h-auto w-60 object-contain" />
			</Link>
		</div>
	</div>
</div>
