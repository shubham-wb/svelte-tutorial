<script lang="ts">
  const { counter = { count: "b mystery" } } = $props();
</script>

<h2>Nested Counter: {counter.count}</h2>
