<script context="module">
    let totalCount = 0;
    export function getTotalCount(){
        return totalCount
    } 

</script>
<script>
    let count = 0;
    function handleClick(){
        count += 1;
        totalCount = totalCount + 1
    }
</script>

<button on:click={handleClick}>counte - {count}</button>