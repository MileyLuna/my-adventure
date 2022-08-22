<script>
    import Secret from "./Secret.svelte";
    import Movie from "./Movie.svelte";
    import ProjectItem from "./ProjectItem.svelte";
    export let showPro = false;

    let items = [
        { label: "Secret Stash", value: 1, component: Secret },
        { label: "Movie Saga", value: 2, component: Movie },
    ];
</script>

{#if showPro}
    <ProjectItem {items} on:click />
{/if}
