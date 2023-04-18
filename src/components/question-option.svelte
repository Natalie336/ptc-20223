<script>
	import { createEventDispatcher } from 'svelte';
	export let letter = 'a';
	export let text = '';
	export let selected = false;
	const dispatch = createEventDispatcher();
	function clicked() {
		dispatch('clicked');
	}
</script>

<button class="answer {selected ? 'selected' : ''}" on:click={clicked}>
	<div class="check" data-letter={letter.toUpperCase()} />
	<span>{text}</span>
</button>

<style>
	.answer {
		background-color: unset;
		height: 72px;
		border: 2px solid var(--color-purple);
		display: grid;
		grid-template-columns: auto 1fr;
		align-items: stretch;
		gap: 12px;
		padding: 0;
		cursor: pointer;
	}
	.answer.selected {
		background-color: var(--color-purple);
		color: white;
	}
	.answer:focus-visible {
		outline: 2px solid var(--color-purple);
		outline-offset: 1px;
	}
	.answer > span {
		display: flex;
		align-items: center;
		justify-content: start;
		font-size: 1rem;
		padding: 4px 8px;
	}
	.check {
		width: 60px;
		background-color: var(--color-purple);
		position: relative;
	}
	.check::before {
		content: attr(data-letter);
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		font-size: 2rem;
		font-weight: bold;
		color: white;
	}
	.answer.selected .check {
		background-color: white;
		border: 4px solid var(--color-purple);
	}
	.answer.selected .check::before {
		color: var(--color-purple);
	}
</style>