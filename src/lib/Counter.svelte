<script lang="ts">
  let count: number = $state(0);
  const increment = () => {
    count += 1;
  };

  let title = "Hello Shubham";
</script>

<button onclick={increment}>
  count is {count}
</button>
<h1>
  {title}
</h1>
