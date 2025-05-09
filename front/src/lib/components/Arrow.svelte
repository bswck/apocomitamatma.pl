<script>
	// @ts-nocheck
	import src from '$lib/images/decorations/arrow1.gif';

	let { direction = 'up', scale = '1', class: classes = '' } = $props();

	const rotations = {
		up: 'rotate(0deg)',
		right: 'rotate(90deg)',
		down: 'rotate(180deg)',
		left: 'rotate(-90deg)'
	};
</script>

<img {src} alt="" style="scale: {scale}; width: auto; height: auto;" class={classes} />
