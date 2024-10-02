<script>
    import DevIcon from './DevIcon.svelte';
    
    // Icons used from devicon.dev
    const techs = [
        "cplusplus",
        "rust",
        "python",
        "html5",
        "css3",
        "markdown",
        "vuejs",
        "svelte",
        "tailwindcss",
        "dotnetcore",
        "qt",
        "git",
        "github",
        "linux",
        "bash",
        "powershell"
    ];

</script>

<div class="mb-auto mt-4 md:m-0 inline-flex flex-wrap rounded-xl place-center w-1/2 h-1/2 border-4 p-2 shadow-lg">
    {#each techs as icon}
    <div class="w-1/4 h-1/4 p-2 md:p-0.5 lg:p-1 hover:p-0 md:w-1/5 md:h-1/5 m-auto">
        <DevIcon {icon} />
    </div>
    {/each}
</div>

<style>
    div {
        border-color: var(--raisin-black);
    }
</style>