<script>
	/** @type{{url: string, class?: string, newTab?: boolean, children: import("svelte").Snippet}} */
	let { url, class: classes, newTab, children, ...others } = $props();

	const newTabArgs = newTab ? { target: '_blank', rel: 'noopener noreferrer' } : {};
</script>

<a
	href={url}
	aria-label="link"
	{...newTabArgs}
	class="transition-all hover:scale-110 {classes}"
	{...others}
>
	{@render children()}
</a>
