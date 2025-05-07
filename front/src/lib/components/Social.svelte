<script>
	import Icon from '@iconify/svelte';
	import Link from './Link.svelte';

	/** @type{any & {
	 * platform: "youtube" | "discord" | "tiktok" | "facebook",
	 * children?: import("svelte").Snippet,
	 * }}
	 * */
	let { platform, children, icon, ...others } = $props();

	const platforms = {
		youtube: { url: '/youtube', icon: 'fa-brands:youtube' },
		discord: { url: '/discord', icon: 'fa-brands:discord' },
		tiktok: { url: '/tiktok', icon: 'fa-brands:tiktok' },
		facebook: { url: '/facebook', icon: 'fa-brands:facebook' }
	};

	/** @type{{url: string, icon: string}} */
	// @ts-ignore
	const { url, icon: defaultIcon } = platforms[platform];
	if (!icon) {
		icon = defaultIcon;
	}
</script>

<Link {url}>
	{#if children}
		{@render children()}
	{:else}
		<Icon {icon} {...others} />
	{/if}
</Link>
