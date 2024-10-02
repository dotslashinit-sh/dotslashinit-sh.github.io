<script lang="ts">
    import SimpleIcon from './SimpleIcon.svelte'

    export let icon: string;
    export let url: string;
</script>

<div class="p1">
    <a href="{url}" target="_blank" class="flex flex-row place-items-center">
        <div class="w-12 h-12 m-2">
            <SimpleIcon {icon}/>
        </div>
        <slot/>
    </a>
</div>

<style>
    a {
        font-family: 'Zilla Sans', sans-serif;
        font-weight: normal;
        text-align: center;
    }

    a:hover {
        font-weight: bold;
        text-decoration: underline;
    }

    div > a > div {
        transition: 0.2s cubic-bezier(0.25, 0.46, 0.45, 0.94);
    }

    div:hover > a > div {
        transition: 0.2s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        padding: 0.2rem;
    }
</style>