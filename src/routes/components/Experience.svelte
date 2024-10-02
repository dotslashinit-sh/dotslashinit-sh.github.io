<script>
    import ExpCard from './ExpCard.svelte'
    import ExpSection from './ExpSection.svelte'
</script>

<ExpSection title="Web Development">
    <ExpCard icons={["html5", "css3"]} tech="HTML5 / CSS3">
        <p slot="exp">Responsive web design, animations, vector graphics</p>
    </ExpCard>
    <ExpCard icons={["javascript", "typescript"]} tech="Javascript / Typescript">
        <p slot="exp">Language basics, DOM, JSON, networking, NodeJS, Deno, parallel programming.</p>
    </ExpCard>
    <ExpCard icons={["svelte", "vuejs", "tailwindcss"]} tech="Frameworks">
        <p slot="exp">Responsive web design with svelte and vue, native applications using Tauri and Rust</p>
    </ExpCard>
</ExpSection>

<ExpSection title="Native development">
    <ExpCard icons={["c", "cplusplus", "qt"]} tech="C/C++">
        <p slot="exp">C++20, memory management, OOPS, RTTI, Boost C++ libraries, Qt framework.</p>
        <ol slot="proj">
            <li><a href="https://github.com/dotslashinit-sh/music-visualizer" target="_blank">Music Visualizer</a></li>
            <li><a href="https://github.com/dotslashinit-sh/snake-game" target="_blank">Snake Game</a></li>
            <li><a href="https://github.com/dotslashinit-sh/RT-in-a-weekend" target="_blank">Raytracer</a></li>
            <li class="inactive">Covid-19 Tracker (GUI)</li>
        </ol>
    </ExpCard>
    <ExpCard icon="rust" tech="Rust">
        <p slot="exp">Rust 2021 edition, basics, generics, network sockets, native API, integration with C/C++</p>
    </ExpCard>
    <ExpCard icon="dotnetcore" tech=".NET/C#">
        <p slot="exp">C# 10, .NET Standard Library, OOPS, , network programming, parallel programming.</p>
    </ExpCard>
</ExpSection>

<ExpSection title="Platforms and Tools">
    <ExpCard icons={["windows11", "powershell"]} tech="Windows">
        <p slot="exp">Windows development with .NET and C/C++, Powershell, Powershell scripting.</p>
    </ExpCard>
    <ExpCard icons={["linux", "bash"]} tech="Linux">
        <p slot="exp">Linux command line (GNU), grep, awk, vim, bash scripting.</p>
    </ExpCard>
    <ExpCard icons={["android", "kotlin"]} tech="Android">
        <p slot="exp">Android development with Kotlin, UI/UX with compose.</p>
    </ExpCard>
    <ExpCard icons={["visualstudio", "vscode", "androidstudio", "neovim"]} tech="Other tools">
        <p slot="exp">Visual Studio 2022, Visual Studio Code, Android Studio, Neovim.</p>
    </ExpCard>
</ExpSection>

<style>
    li, p {
        font-size: 1.25rem;
        font-weight: 450;
    }

    p {
        max-width: 20vw;
        text-align: center;
    }

    a:hover {
        font-weight: 550;
    }

    .inactive {
        text-decoration: line-through;
        opacity: 80%;
    }

    ol {
        list-style: lower-greek;
    }
</style>