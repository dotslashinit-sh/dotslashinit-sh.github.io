<script lang="ts">
    export let title: string;
</script>

<div class="min-w-full flex flex-col place-items-center">
    <h1>{title}</h1>
    <div class="p-12 m-auto flex flex-row flex-wrap space-x-4 gap-y-4 justify-center">
        <slot />
    </div>
</div>

<style>
    h1 {
        font-size: 2.5rem;
        font-weight: bolder;
        text-decoration: underline;
    }
</style>