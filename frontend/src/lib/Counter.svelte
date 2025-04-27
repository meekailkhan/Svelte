<script>
    let count = 0;

    function handleClick(event,stepSize){
        console.log(event)  
        count+=stepSize
    }
</script>

<div>
    <button on:click={()=> {count = count + 1}}>{count}</button>
    <button on:click={(event) => handleClick(event,5)}>{count}</button>
    
</div>