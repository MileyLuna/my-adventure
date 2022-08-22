<script>
    export let showAbout = false;

</script>

{#if showAbout}
    <div class="backdrop"  on:click>
        <div  class="modal">
            <h2>About me:</h2>
            <h3>Degree Change:</h3>
            <p>
                I come from a career background in Healthcare. The original goal
                was to become a Occupational Therapist to physically heal and
                imporve humans. However, through job shadowing I figured it was
                not the right path for me.
            </p>
            <h3>Career Change:</h3>
            <p>
                One month before graduation From UW - River Falls, I recieved an
                offer with Optum and took the opportunity. The role required
                multiple system usage and the frustration of it sparked my
                curiosity in Software development.
            </p>
            <h3>Scavanger Hunt & Currently:</h3>
            <p>
                On a software development/engineer scvanger hunt, I found Prime
                Digital Academy Full Stack BootCamp and took the great
                opportunity through MSP Hire Tech funding. Definetly a hate,
                love relationship with coding - It's been very intense and
                memerising.
            </p>
            <h3>Future:</h3>
            <p>
                I hope to continue being in the carrer field I fell deeply for -
                Healthcare.
            </p>
        </div>
    </div>
{/if}

<style>
    .backdrop {
        width: 100%;
        height: 100%;
        position: fixed;
        background: rgba(0, 0, 0, 0.8);
    }
    .modal {
        padding: 10px;
        border-radius: 10px;
        max-width: 400px;
        margin: 10% auto;
        text-align: center;
        background: rgb(252, 233, 233);
    }

</style>
