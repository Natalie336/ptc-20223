<script>
	export let answer = false;
</script>

{#if answer}

<p style="color: green;"> 
		Great job - that was the answer! 
</p>
	
{:else}
	
	<p style="color: red;">
		oh man, that answer wasn't quite right...
	</p>
{/if}


