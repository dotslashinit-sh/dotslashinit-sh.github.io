<script>
    import '../app.css'
    
</script>

<div class="flex content-center flex-col">
    <slot></slot>
</div>

<style>
    div {
        width: 100%;   
        /* Color palette */
        --ghost-white: #e8e9f3ff;
        --silver: #cececeff;
        --french-gray: #a6a6a8ff;
        --raisin-black: #272635ff;
        --non-photo-blue: #b1e5f2ff;

        background-color: var(--ghost-white);
        font-family: 'Zilla Slab', sans-serif;
        color: var(--raisin-black);
    }
</style>