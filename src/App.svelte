<script>
  import { roll } from "./utils.js";

  let promise = $state(roll());
</script>

<button onclick={() => (promise = roll())}> roll the dice </button>
{#await promise}
  <p>...rolling</p>
{:then number}
  <p>You rolled a {number}!</p>
{:catch}
  <p>There was an error rolling the dice.</p>
{/await}
