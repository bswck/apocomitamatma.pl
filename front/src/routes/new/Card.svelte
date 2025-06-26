<script>
	let { children, class: classes = '' } = $props();
</script>

<div
	class="border-(--color-outline) border-3 flex w-full flex-col items-center gap-6 rounded-2xl p-4 {classes}"
>
	{@render children()}
</div>
