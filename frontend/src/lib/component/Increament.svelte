<script>
  import { count } from "../../store/stores";

    function increament(){
        count.update(value =>{
            return value + 1
        })
    }
</script>

<button on:click={increament}>Increament</button>