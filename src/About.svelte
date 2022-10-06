<script>
</script>

<main>
    <div class="modal">
        <p id="one">
            My original goal was to become an Occupational Therapist to
            physically improve a human activity of daily living - hence my
            previous careers in direct patient care. However, through job
            shadowing I figured it was not the right path for me. I want a
            dynamic workflow that provides continuos growth.
        </p>
        <p id="two">
            One month before graduation from UW - River Falls, I took an
            opportunity with Optum Advocacy Department. The role required
            multiple system usage and the frustration of it sparked my curiosity
            in software development.
        </p>
        <p id="three">
            During the software development/engineer learning scvanger hunt, I
            found Prime Digital Academy Full Stack BootCamp and took the great
            opportunity through MSP Hire Tech. The Bootcamp was like a marriage;
            full of hate and love. It was truly a wonderful, intense, and
            memerising experience where I gained new friendship, knowledge, and
            a new me.
        </p>
        <p id="four">
            I am seeking for a work environment that will enable my growth in
            software development and it's lifecycle, also guidiance in
            using industries best pratices and incorperating accessibility
            fundamentals.
        </p>
    </div>
</main>

<style>
    main {
        width: 100%;
        margin: auto;
        text-align: center;
        height: 100%;

    }
    div {
        margin: 5rem 0rem 0rem 20rem;
        max-width: 60%;
        height: 100%;
    }

    p {
        line-height: 1.75em;
        border-top: 3px solid black;
        margin: 0;
        padding: 30px 50px 30px 50px;
        position: relative;
    }
    #one,
    #three {
        border-right: 3px solid black;
    }
    #one::before {
        content: "Degree";
        left: 100%;
        margin-left: -20px;
    }
    #two,
    #four {
        border-left: 3px solid black;
    }
    #two::before {
        content: "Career";
        right: 100%;
        margin-right: -20px;
    }
    #three {
        border-right: 3px solid black;
    }
    #three::before {
        content: "Hunt";
        left: 100%;
        margin-left: -20px;
    }

    #four::before {
        content: "Goals";
        right: 100%;
        margin-right: -20px;
    }

    p::before {
        border-radius: 50%;
        position: absolute;
        height: 2em;
        width: 4em;
        line-height: 1em;
        background-color: grey;
        color: #34435e;
        padding-top: 10px;

    }
    p:first-child {
        border-top: 0;
    }
</style>
