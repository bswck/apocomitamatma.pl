<script>
	import { browser } from '$app/environment';
	import * as formulasMap from '$lib/images/decorations/formulas.js';

	const formulas = Object.values(formulasMap);

	const positions = [
		{ x: 7, y: 12, scale: 3.2, opacity: 0.22 },
		{ x: 48, y: 9, scale: 2.9, opacity: 0.28 },
		{ x: 93, y: 14, scale: 3.5, opacity: 0.32 },
		{ x: 10, y: 47, scale: 4.1, opacity: 0.18 },
		{ x: 50, y: 52, scale: 3.7, opacity: 0.35 },
		{ x: 90, y: 48, scale: 2.8, opacity: 0.25 },
		{ x: 12, y: 87, scale: 3.0, opacity: 0.19 },
		{ x: 53, y: 91, scale: 3.3, opacity: 0.3 },
		{ x: 94, y: 86, scale: 3.6, opacity: 0.22 }
	];

	let scrollY = 0;
	let parallaxBase = 0;

	if (browser) {
		scrollY = window.scrollY;
		parallaxBase = scrollY;

		window.addEventListener('scroll', () => {
			scrollY = window.scrollY;
		});
	}
</script>

<div class="pointer-events-none absolute left-0 top-0 -z-10 h-full w-full overflow-hidden">
	{#each formulas as src, i}
		<img
			{src}
			alt=""
			style="
				position: absolute;
				left: {positions[i].x}%;
				top: calc({positions[i].y}% + {(scrollY - parallaxBase) * 0.2}px);
				transform: scale({positions[i].scale});
				width: 4rem;
				height: auto;
				filter: opacity({positions[i].opacity});
			"
			class="transition-transform duration-[0ms] will-change-transform"
		/>
	{/each}
</div>
