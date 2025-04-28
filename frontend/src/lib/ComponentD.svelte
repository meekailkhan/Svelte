<script>
    import {getContext} from 'svelte'
    let username = getContext('username');
</script>


<div>
    <h2>Component D</h2>
    <h2>{username}</h2>
</div>