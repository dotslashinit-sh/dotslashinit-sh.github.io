<svelte:head>
    <title>Dot's page</title>
</svelte:head>

<script>
    import HelloText from './components/HelloText.svelte'
    import Tech from './components/Tech.svelte'
    import Experience from './components/Experience.svelte'
    import Contact from './components/Contact.svelte'
</script>

<section id="greeting" class="flex flex-col justify-center md:grid md:grid-cols-2">
    <HelloText />
    <Tech />
</section>

<section id="about">
    <div class="grid grid-flow-row">
        <Experience />
    </div>
</section>

<section id="socials" class="place-items-center flex flex-col">
    <Contact />
</section>

<style>
    section {
        min-height: 100vh;
        place-items: center;
    }
</style>