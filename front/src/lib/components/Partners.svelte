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
		<Link url="/showcase" newTab={true}>-> Zobacz przykładowe lokowania</Link>
		<div class="flex flex-row gap-4">
			<img src={NowaEra} alt="Nowa Era" class="w-46 h-auto object-cover" />
			<img src={PWN} alt="PWN" class="w-46 h-auto object-contain" />
		</div>
		<div class="flex flex-col gap-4 md:flex-row">
			<img src={SWPS} alt="SWPS" class="w-46 h-auto object-contain" />
			<img src={WSKZ} alt="WSKZ" class="w-46 h-auto object-contain" />
		</div>
	</div>
</div>
