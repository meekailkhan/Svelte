<script>
  let name = ["meekail", "mujaahid", "arbaaz", "mahir"];
</script>

<ul>
  {#each name as person, i}
    <li>{i + 1}. {person.toUpperCase()}</li>
  {/each}
</ul>
