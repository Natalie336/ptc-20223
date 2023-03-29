<script>
    export let Anwser = false;
</script>

{#if answer}

<p>
    Great job - that was the answer!
</p>

<p>
    oh man, that answer wasn't quite right...
</p>
{/if}

<script>
    export let Answer = true;
</script>

{#if answer}

<p>
    Great job - that was the answer!
</p>

<p>
    oh man, that answer wasn't quite right...
</p>
{/if}
