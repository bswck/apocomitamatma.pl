<script>
	let { children, class: classes = '' } = $props();
</script>

<div class="w-full flex-col flex items-center gap-6 {classes}">
    {@render children()}
</div>