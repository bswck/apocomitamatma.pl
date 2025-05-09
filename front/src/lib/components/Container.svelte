<script>
	let { children, class: classes = '' } = $props();
</script>

<div
	class="
    mx-auto flex w-full max-w-7xl flex-col items-center
    justify-between gap-8 px-10 text-center
    xl:flex-row
    {classes}
    "
>
	{@render children()}
</div>
