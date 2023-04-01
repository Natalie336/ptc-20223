<script>
	export let answer = false;
</script>

{#if answer}

<div style="color: green;"> 
		Great job - that was the answer! 
</div>
	
{:else}
	
	<div style="color: red;">
		oh man, that answer wasn't quite right...
	</div>
{/if}
