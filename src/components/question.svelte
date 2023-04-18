<script>
   import Answer from './answer.svelte';
   import QuestionOption from './question-option.svelte';
 
   export let number = 1;
    

   /** @type { [string, string] | [string, string, string] | [string, string, string, string] } */
	export let answers = ['', ''];

    /** @type { 0 | 1 | 2 | 3 | null } */
	export let correctIndex = 0;
	/** @type { number } */
	let selected;

</script>

<div>
    
    <p style="font-size: 1.5rem; margin-top: 0;">{number}. <b><slot /></b></p>

	<div class="answer-group">
		{#each answers as answer, index}
			<QuestionOption
				letter={['a', 'b', 'c', 'd'][index]}
				text={answer}
				selected={selected == index}
				on:clicked={() => (selected = index)}
			/>
		{/each}
	</div>
</div>

<Answer answer={correctIndex == selected} />

<style>
	.answer-group {
		display: grid;
		gap: 24px;
	}
</style>

