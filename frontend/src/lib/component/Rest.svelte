<script>
  import { count } from "../../store/stores";

    function resetVal(){
        count.set(0)
    }
</script>

<button on:click={resetVal}>Reset</button>