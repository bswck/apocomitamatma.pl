<script>
	let { children, id, class: classes = '' } = $props();
</script>

<section
	{id}
	class="
    border-t-1 border-t-(--color-outline) relative
    flex w-full grow flex-col items-center
    justify-center {classes}
    "
>
	{@render children()}
</section>
