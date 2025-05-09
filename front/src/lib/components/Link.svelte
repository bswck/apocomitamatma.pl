<script>
	/** @type{{url: string, class?: string, newTab?: boolean, children: import("svelte").Snippet}} */
	let { url, class: classes, newTab, children } = $props();

	const newTabArgs = newTab ? { target: '_blank', rel: 'noopener noreferrer' } : {};
</script>

<a href={url} aria-label="link" {...newTabArgs} class="hover:brightness-80 {classes}">
	{@render children()}
</a>
