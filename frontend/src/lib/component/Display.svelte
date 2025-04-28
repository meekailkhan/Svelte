<script>
  import { onDestroy } from "svelte";
  import { count,time,customCount } from "../../store/stores";
  import Decreament from "./Decreament.svelte";
  import Increament from "./Increament.svelte";
  import Rest from "./Rest.svelte";

  const dateFormatter = new Intl.DateTimeFormat('en',{
    hour12 : true,
    hour : "numeric",
    minute : "2-digit",
    second : "numeric"
  });

    // let counter;
    // const unsubscribe = count.subscribe(value =>{
    //     counter = value
    // });
    // onDestroy(unsubscribe)
</script>

<!-- <h2>current count is = {counter}</h2> -->
 <h2>the current time is - {dateFormatter.format($time)}</h2>

<h2>current count is = {$count}</h2>

<Increament />
<Decreament />
<Rest />

 <hr>
<button on:click={()=> customCount.increment()}>Increament</button>
<button on:click={()=> customCount.decrement()}>Decreament</button>
<button on:click={()=> customCount.increment(5)}>Increament 5</button>
<button on:click={()=> customCount.decrement(5)}>Decreament 5</button>

<button on:click={()=> customCount.reset()}>Reset</button>

<h2>custom count is - {$customCount}</h2>