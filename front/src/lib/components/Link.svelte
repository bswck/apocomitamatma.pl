<script>
	/** @type{{url: string, class?: string, children: import("svelte").Snippet}} */
	let { url, class: classes, children } = $props();
</script>

<a
	href={url}
	aria-label="link"
	target="_blank"
	rel="noopener noreferrer"
	class="hover:brightness-80 {classes}"
>
	{@render children()}
</a>
