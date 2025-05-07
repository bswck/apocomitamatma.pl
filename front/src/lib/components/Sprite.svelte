<script>
	import { onMount } from 'svelte';
	import * as sprites from './spriteImages';

	/** @type{{which: 'delta' | 'figures' | 'rizz', class?: string}}*/
	let { which, class: classes } = $props();

	/** @type {HTMLImageElement} */
	let image;
</script>

<img bind:this={image} src="src/lib/images/sprites/{which}.png" class={classes} alt="" />
