<script>
    import DiPostgresql from "svelte-icons/di/DiPostgresql.svelte";
    import DiReact from "svelte-icons/di/DiReact.svelte";
    import DiJavascript1 from "svelte-icons/di/DiJavascript1.svelte";
    import DiVisualstudio from "svelte-icons/di/DiVisualstudio.svelte";
    import DiNodejsSmall from "svelte-icons/di/DiNodejsSmall.svelte";
    import DiGithubBadge from "svelte-icons/di/DiGithubBadge.svelte";
    import DiHtml5 from "svelte-icons/di/DiHtml5.svelte";
    import DiCss3 from "svelte-icons/di/DiCss3.svelte";
</script>

<main>
    <div class="container">
        <div class="contact-container">
            <h2>Get In Touch</h2>
            <p>
                I am actively looking for software developer role, also open to
                collaboration, and freelance work.
                <br />
                Otherwise don't be shy to send me a quick Hello. And I am always
                open to opportunity for growth, so feel free to send over tips, suggestions,
                and/or resources.
            </p>
            <br>
            <a class="email-link" href="mailto:vangmaihlee@ymail.com"
                >Say Hello</a
            >
        </div>

        <div class="tool-container">
            <p>My Toolbox:</p>

            <div class="icon-container">
                <div class="icon-box">
                    <div class="icon">
                        <DiHtml5 />
                    </div>
                    <p>HTML</p>
                </div>
                <div class="icon-box">
                    <div class="icon">
                        <DiCss3 />
                    </div>
                    <p>CSS</p>
                </div>
                <div class="icon-box">
                    <div class="icon">
                        <DiJavascript1 />
                    </div>
                    <p>JavaScript</p>
                </div>
                <div class="icon-box">
                    <div class="icon">
                        <DiReact />
                    </div>
                    <p>React.js</p>
                </div>
                <div class="icon-box">
                    <div class="icon">
                        <DiNodejsSmall />
                    </div>
                    <p>Node.js</p>
                </div>
                <div class="icon-box">
                    <div class="icon">
                        <DiPostgresql />
                    </div>
                    <p>Postgres</p>
                </div>
                <div class="icon-box">
                    <div class="icon">
                        <DiGithubBadge />
                    </div>
                    <p>GitHub</p>
                </div>
                <div class="icon-box">
                    <div class="icon">
                        <DiVisualstudio />
                    </div>
                    <p>Visual Studio</p>
                </div>
            </div>
        </div>
    </div>
</main>

<style>
    main {
        color: grey;
        line-height: 1.5em;
        height: 100%;
    }
    .contact-container {
        width: 80%;
    }
    .email-link {
        cursor: pointer;
        border: 1px solid rgb(114, 114, 114);
        padding: 1rem 1rem;
        border-radius: 8px;
        text-decoration: none;
        color: grey;
        width: 20%;
    }
    a{
        margin-top: 3rem;
    }
    .email-link:hover {
        background-color: rgb(195, 141, 141);
    }

    .container {
        width: 40%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin: auto;
        text-decoration-skip-ink: none;
        background-color: rgba(201, 76, 76, 0.3);
        height: 100%;
    }
    .icon-container {
        width: 60%;
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        align-content: space-between;
    }

    .tool-container {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin-top: 3rem;

    }
    .icon {
        width: 72px;
        height: 72px;
    }
</style>
