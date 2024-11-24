<script lang="ts">
	import TypewriterEffectSmooth from '$lib/ui/TypewriterEffect/TypewriterEffectSmooth.svelte';
	
	const words = [
		{
			text: 'Make'
		},
		{
			text: 'the'
		},
		{
			text: 'best'
		},
		{
			text: 'web-apps'
		},
		{
			text: 'with.'
		},
		{
			text: '@MooseCoding',
			className: 'text-purple-500 dark:text-blue-500'
		}
	];
</script>

<div class="flex h-[40rem] flex-col items-center justify-center">
	<TypewriterEffectSmooth {words} />
</div>