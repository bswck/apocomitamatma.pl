<script>
	let { children, class: classes = '' } = $props();
</script>

<div
	class="
    mx-auto flex w-full max-w-7xl flex-col items-center
    justify-between px-10 text-center
    lg:flex-row
    {classes}
    "
>
	{@render children()}
</div>
