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
        <div class="inner-container">
            <h2>Hire Me!</h2>
            <p>
                I am actively looking for full-time back-end software developer
                role. And no, I don't dislike the front-end I am just not as
                artistic. I don't mind the entire (full-stack) process.
                <br />
                I am also open collaboration and freelance work.
                <br />
                <br />
                Toolbox of skill sets and language aquired: 
            </p>
        </div>

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

        <div>
            <p></p>
            <div class="email-link">
                <a href="mailto:vangmaihlee@ymail.com">Say Hello</a>
            </div>
        </div>
    </div>
</main>

<style>
    main {
        color: grey;
        line-height: 1.50em;
        height: 100%;
    }
    .email-link {
        cursor: pointer;
        border: 1px solid rgb(114, 114, 114);
        padding: 1rem 1rem;
        border-radius: 8px;
        text-decoration: none;
        color: grey;
        margin-top: 2rem;
        width: 20%;
    }
    .email-link:hover {
        background-color: rgb(195, 141, 141);
    }

    .container {
        width: 40%;
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: auto;
        text-decoration-skip-ink: none;
        background-color: rgba(201, 76, 76, 0.3);
        height: 100%;
        justify-content: center;
        /* padding: 4rem 0rem 4rem 0rem; */
        /* margin-top: 10rem; */
    }
    .inner-container {
        width: 80%;
    }
    .icon-container {
        width: 60%;
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        align-content: space-between;
        justify-content: center;
        margin-top: 1rem;
    }
    .icon {
        width: 72px;
        height: 72px;
    }
</style>
