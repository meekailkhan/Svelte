<script>
    import TabA from "./TabA.svelte";
    import TabB from "./TabB.svelte";
    import TabC from "./TabC.svelte";

    let activeTab = TabC

</script>

<div>
    <button on:click={()=> activeTab = TabA}>Tab A</button>
    <button on:click={()=> activeTab = TabB}>Tab B</button>
    <button on:click={()=> activeTab = TabC}>Tab C</button>

    <svelte:component this={activeTab}></svelte:component>

</div>