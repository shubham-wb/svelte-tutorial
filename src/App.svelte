<script>
  let numbers = $state([1, 2, 3, 4]);

  function addNumber() {
    numbers[numbers.length] = numbers.length + 1;
  }

  let total = $derived(numbers.reduce((a, b) => a + b, 0));

  $inspect(numbers, "Numbers array").with(console.trace);
</script>

<p>{numbers.join(" + ")} = {total}</p>

<button onclick={addNumber}> Add a number </button>
