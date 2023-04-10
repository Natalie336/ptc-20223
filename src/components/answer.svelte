<script>
	export let answer = false;
</script>

{#if answer}

<p class="correct"> 
		Great job - that was the answer! 
</p>
	
{:else}
	
	<p class="incorrect">
		oh man, that answer wasn't quite right...
	</p>
{/if}




.correct {
	color= green;
}

.incorret {
	color= red;
}
