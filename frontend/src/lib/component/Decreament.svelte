<script>
  import { count } from "../../store/stores";

    function decreament(){
        count.update(val =>{
            return val -1
        })
    }
</script>

<button on:click={decreament}>Decreament</button>