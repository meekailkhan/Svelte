<script>
  import PopUp from "./PopUp.svelte";

    let showPopUp = false;
    function handleClose(e){
        showPopUp = false
        console.log(e)
    }
</script>

<div>
    <button on:click={()=> showPopUp = true}>Show Pop Up</button>
    {#if showPopUp}
    <PopUp on:close={handleClose}/>
    {/if}
</div>