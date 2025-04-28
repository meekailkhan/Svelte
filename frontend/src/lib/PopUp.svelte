<script>
    import {createEventDispatcher} from 'svelte'
    const dispatch = createEventDispatcher();
</script>

<div>
    <div>Pop Up Component</div>
    <button on:click={()=> dispatch("close","meekail")}>Close Pop Up</button>
</div>