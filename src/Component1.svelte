<script>
  export let items = [];
</script>

<style>
  ul {
    padding: 0;
    margin: 0;
    list-style: none;
  }

  li {
    color: rebeccapurple;
  }

  li:nth-child(even) {
    color: #998033;
  }
</style>

<ul>
  {#each items as item}
    <li>
      <slot item={item}>{item}</slot>
    </li>
  {/each}
</ul>
