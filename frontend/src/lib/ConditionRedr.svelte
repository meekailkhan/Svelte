<script>
   let num = 1;
</script>

<div>
    {#if num === 0}
    <h1>the number is zero</h1>
    {:else if num > 0}
    <h1>the number is greaterthen zero</h1>
    {:else if num < 0}
    <h1>the number is lessthen zero</h1>
    {:else}
    <h1>this is not a number</h1>
    {/if}
</div>

<style>

</style>