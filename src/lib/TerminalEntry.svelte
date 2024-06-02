<script lang="ts">
	import type { TerminalEntry } from '$lib/terminalEntry';

	let { entry }: { entry: TerminalEntry } = $props();
	let parsedText: (string | { bold: boolean; text: string })[] = $state(parseText(entry.text));

	function parseText(text: string) {
		const regex = /\*\*([a-zA-Z0-9:-]+)\*\*/g;
		const parts = [];
		let lastIndex = 0;

		for (const match of text.matchAll(regex)) {
			const before = text.slice(lastIndex, match.index);
			if (before) {
				parts.push(before);
			}

			parts.push({ bold: true, text: match[1] });
			lastIndex = match.index + match[0].length;
		}

		const after = text.slice(lastIndex);
		if (after) {
			parts.push(after);
		}

		return parts;
	}
</script>

<div
	class="mb-1 overflow-x-hidden whitespace-pre-wrap rounded px-0.5 {entry.type === 'command'
		? 'text-blue-400'
		: 'text-green-400'}"
>
	{#each parsedText as part}
		{#if typeof part === 'string'}
			{part}
		{:else}
			<span class="font-bold">{part.text}</span>
		{/if}
	{/each}
</div>
