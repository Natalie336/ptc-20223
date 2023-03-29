<script>
    export let anwser = false;
</script>

{#if answer}

<p>
    Great job - that was the answer!
</p>
{:else}
<p>
    oh man, that answer wasn't quite right...
</p>
{/if} 
