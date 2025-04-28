<script>
  import ComponentB from "./ComponentB.svelte";
  import {setContext} from 'svelte'

  let username = "this is username";

  setContext("username",username)

</script>

<div>
    <h1>component A</h1>
    <ComponentB />
</div>