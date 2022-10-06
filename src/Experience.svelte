<script>
    import Software from "./Software.svelte";
    import CnaC from "./CnaC.svelte";
    import CnaG from "./CnaG.svelte";
    import Marketing from "./Marketing.svelte";
    import English from "./English.svelte";
    import Hca from "./Hca.svelte";
    import ExperienceItem from "./ExperienceItem.svelte";
    import Rca from "./Rca.svelte";

    // export let showExp = false;

    let items = [
        { label: "Prime Digital Academy", value: 1, component: Software },
        { label: "Optum", value: 2, component: Hca },
        { label: "Gillete Childrens", value: 3, component: CnaG },
        { label: "Cerenity Senior Care", value: 4, component: CnaC },
        { label: "Our House Senior Living", value: 5, component: Rca },
        { label: "Second Harvest Heartland", value: 6, component: Marketing },
        { label: "Shih Hsin University", value: 7, component: English },
    ];
</script>

<!-- {#if showExp} -->
<ExperienceItem {items} on:click/>
<!-- {/if} -->

