<script>
    import Secret from "./Secret.svelte";
    import Movie from "./Movie.svelte";
    import ProjectItem from "./ProjectItem.svelte";

    let items = [
        { label: "Secret Stash", value: 1, component: Secret },
        { label: "Movie Saga", value: 2, component: Movie },
    ];


</script>


<main>
    <ProjectItem {items} on:click/>
</main>

<style>

</style>
