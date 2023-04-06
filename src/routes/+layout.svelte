<div class="background">
    <div class="layout">
        <slot />
    </div>
</div>

<style>
    .background {
        padding: 16px;
        
        position: absolute;
        inset: 0;

        background-color:lightblue
    }

    .layout {
        width: 100%;
        max-width: 1024px;
        margin: 0 auto;

    }
</style>

