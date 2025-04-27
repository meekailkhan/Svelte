<script>
  let names = [
    {
      firstName: "clerk",
      lastName: "kent",
    },
    {
      firstName: "bruce",
      lastName: "wayn",
    },
    {
      firstName: "diana",
      lastName: "abcd",
    },
  ];
</script>

<div>
  <ul>
    {#each names as name,i (i)}
      <li>{name.firstName} {name.lastName}</li>
    {/each}
  </ul>
</div>

<style>
</style>
