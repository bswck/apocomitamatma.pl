<script>
	let { children, id, class: classes = '' } = $props();
</script>

<section
	{id}
	class="
    border-t-1 border-t-(--color-outline)
    relative w-full grow items-center
    justify-center {classes}
    "
>
	{@render children()}
</section>
