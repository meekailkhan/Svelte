<script>

import {createEventDispatcher} from 'svelte'

const dispatch = createEventDispatcher()
function handleGreet(e){
    dispatch("greet",'hello')
}


</script>

<button on:click={handleGreet}>Greet</button>