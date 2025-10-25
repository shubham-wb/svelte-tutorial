<script lang="ts">
  import Nested from "./Nested.svelte";
  import { counter } from "./shared.svelte.js";

  function increment() {
    counter.count += 1;
  }
</script>

<h1>Counter: {counter.count}</h1>
<button onclick={increment}>Increment</button>
<Nested {counter} />
