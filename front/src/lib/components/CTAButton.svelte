<script>
	import Icon from '@iconify/svelte';

	/** @type {{ text: string, color: 'red' | 'blue', email: string }} */
	let { text, color, email } = $props();

	const colorClass = color === 'red' ? 'bg-(--color-red)' : 'bg-(--color-blue)';
</script>

<div class="flex flex-col items-center gap-2 text-center">
	<a
		href={`mailto:${email}`}
		class={`inline-flex items-center gap-2 rounded-full px-6 py-3 font-bold text-white shadow-lg transition-all hover:brightness-110 ${colorClass}`}
	>
		<Icon icon="mdi:email-outline" class="text-xl" />
		<span>{text}</span>
	</a>

	<a href={`mailto:${email}`}><p class="text-sm text-white/60">{email}</p></a>
</div>
