<script>
  import ModuleContext,{getTotalCount} from "./ModuleContext.svelte";


</script>

<div>
    <button on:click={()=> alert(getTotalCount())}>Get Total Count</button>
    <ModuleContext />
    <ModuleContext />
    <ModuleContext />

</div>