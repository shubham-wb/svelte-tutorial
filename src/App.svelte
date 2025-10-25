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
<Nested />

{#if counter.count > 30}
  <p>{counter.count} is greater than 30</p>
{:else if counter.count < 21}
  <p>{counter.count} is less than 21</p>
{:else}
  <p>{counter.count} is between 21 and 30</p>
{/if}
