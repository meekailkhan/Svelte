<script>
    let volume = 0;

    $: if(volume < 0){
        alert("Can't go lower")
        volume = 0
    }
    else if(volume > 20){
        alert("Max Volume is 20")
        volume = 20
    }

</script>

<div>
    <button on:click={()=> volume += 2}>Increas Volume</button>
    <button on:click={()=> volume -= 2}>Decrease Volume</button>

    <h2>{volume}</h2>
</div>