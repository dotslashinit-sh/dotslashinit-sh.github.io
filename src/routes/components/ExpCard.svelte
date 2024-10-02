<script lang="ts">
    import DevIcon from './DevIcon.svelte'
    export let icon: string | null = null;
    export let icons: Array<string> | null = null;
    export let tech: string;

    if(icon != null) {
        icons = [icon];
    }
</script>

<div class="rounded-xl border-4 p-4 flex flex-col place-items-center border-slate-600">
    {#if icons != null}
    <div class="inline-flex flex-row space-x-2">
        {#each icons as icon}
        <div class="w-8 h-8">
            <DevIcon icon="{icon}"/>
        </div>
        {/each}
    </div>
    {/if}
    <h2>{tech}</h2>
    {#if $$slots.exp}
        <h3>Experience</h3>
        <slot name="exp" />
    {/if}
    {#if $$slots.proj}
        <h3>Projects</h3>
        <slot name="proj" />
    {/if}
</div>

<style lang="postcss">
    h2 {
        font-size: 1.75rem;
        font-weight: bolder;
        text-decoration: underline;
    }

    h3 {
        font-size: 1.5rem;
        text-decoration: underline;
        font-weight: bold;
    }
</style>