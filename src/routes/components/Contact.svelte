<script lang="ts">
    // Icons from simpleicons.org
    import ContactButton from "./ContactButton.svelte";
</script>

<ul class="flex flex-col md:flex-row md:space-y-0 md:space-x-16">
    <li>
        <ContactButton url="https://github.com/dotslashinit-sh" icon="github">GitHub</ContactButton>
    </li>
    <li>
        <ContactButton url="https://www.hackerrank.com/profile/dotslashconfig" icon="hackerrank">Hackerrank</ContactButton>
    </li>
    <li>
        <ContactButton url="https://www.linkedin.com/in/abhin-raj/" icon="linkedin">LinkedIn</ContactButton>
    </li>
    <li>
        <ContactButton url="mailto:abinr5502@gmail.com" icon="gmail">E-Mail</ContactButton>
    </li>
    <li>
        <ContactButton url="https://discord.com/users/853527642652409866" icon="discord">Discord</ContactButton>
    </li>
</ul>