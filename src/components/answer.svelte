<script>
	export let answer = false;
</script>

{#if answer}

<p class="correct"> 
		Great job - that was the answer! 
</p>
	
{:else}
	
	<p class= "incorrect">
		oh man, that answer wasn't quite right...
	</p>
{/if}

<style>
	.correct, .incorrect {
		font-weight: bold;
		text-decoration: underline;
	}
	.correct {
		color: green;
	}
	.incorrect {
		color: red;
	}
</style>