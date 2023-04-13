<script>
	import Score from "../components/score.svelte";
</script>

<div class="background">
	<div class="layout">
        <div class="header">
            <Score score={0} />
        </div>
        <div class="content">
		    <slot />
        </div>
	</div>
</div>


<style>
	.background {
		padding: 32px;
        display: grid;
		position: absolute;
		inset: 0;

		background-color: var(--color-purple);
	}

	.layout {
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;

        display: grid;
        grid-template-rows: auto 1fr;
        align-items: center;
	}

    .header,.content {
        background-color: white;
        border: 4px solid black;
        padding: 12px 24px;
    }

    .header {
        display: flex;
        justify-content: space-between;
    }
</style>
