<script lang="ts">
	import TerminalEntry from '$lib/TerminalEntry.svelte';
	import type { TerminalEntry as TerminalEntryType } from '$lib/terminalEntry';

	let { content = '' }: { content: TerminalEntryType[] | string } = $props();
</script>

<div class="rounded-lg bg-[#1a1a1a] p-4 font-mono text-green-400 shadow-lg">
	<div class="mb-2 border-b border-gray-700">
		<div class="mb-1 flex space-x-2">
			<div class="h-3 w-3 rounded-full bg-red-500"></div>
			<div class="h-3 w-3 rounded-full bg-yellow-500"></div>
			<div class="h-3 w-3 rounded-full bg-green-500"></div>
		</div>
	</div>
	{#if Array.isArray(content)}
		{#each content as entry}
			<TerminalEntry {entry} />
		{/each}
	{:else}
		<TerminalEntry entry={{ type: 'result', text: content }} />
	{/if}
</div>
