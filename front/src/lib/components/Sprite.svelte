<script>
	import * as sprites from './spriteImages';
	let { which, class: classes } = $props();
	let src = sprites[which];
</script>

<img {src} alt="" class={classes} />
