<script>
	import * as formulasMap from '$lib/images/decorations/formulas.js';

	const formulas = Object.values(formulasMap);

	const positions = [
		{ x: 7, y: 12, opacity: 0.22 },
		{ x: 48, y: 9, opacity: 0.28 },
		{ x: 93, y: 14, opacity: 0.32 },
		{ x: 10, y: 47, opacity: 0.18 },
		{ x: 50, y: 52, opacity: 0.35 },
		{ x: 90, y: 48, opacity: 0.25 },
		{ x: 12, y: 87, opacity: 0.19 },
		{ x: 53, y: 91, opacity: 0.3 },
		{ x: 94, y: 86, opacity: 0.22 }
	];
</script>

<div class="parallax-wrapper">
	{#each formulas as src, i}
		<img
			{src}
			alt=""
			style="
        scale: 1.2;
        left: {positions[i].x}%;
        top: {positions[i].y}%;
        transform: translateZ({-i * 10}px);
        opacity: {positions[i].opacity};
    "
			class="formula"
		/>
	{/each}
</div>

<style>
	.parallax-wrapper {
		position: absolute;
		inset: 0;
		pointer-events: none;
		overflow: hidden;
		z-index: -10;
		transform-style: preserve-3d;
		perspective: 1000px;
	}

	.formula {
		position: absolute;
		width: 4rem;
		height: auto;
		will-change: transform;
	}
</style>
