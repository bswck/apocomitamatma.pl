<script>
	import Icon from '@iconify/svelte';
	import Link from './Link.svelte';

	/** @type {{ text: string, color: 'red' | 'blue', email: string, phoneNumber?: string, class?: string }} */
	let { text, color, email, phoneNumber, class: classes = '' } = $props();

	const colorClass = color === 'red' ? 'bg-(--color-red)' : 'bg-(--color-blue)';
</script>

<div class="flex flex-col items-center gap-3 text-center {classes}">
	<Link
		url={`mailto:${email}`}
		class={`inline-flex items-center gap-2 px-10 py-3 font-bold text-white shadow-lg transition-all hover:brightness-110 ${colorClass}`}
	>
		<Icon icon="mdi:email-outline" class="text-xl" />
		<span class="text-xl">{text}</span>
	</Link>
	<Link url={`mailto:${email}`}><p class="text-md text-white/60">{email}</p></Link>
	{#if phoneNumber}
		<Link url={`tel:${phoneNumber}`} class="text-md text-white/60">
			{phoneNumber}
		</Link>
	{/if}
</div>
