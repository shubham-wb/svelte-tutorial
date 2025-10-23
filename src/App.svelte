<script>
  let numbers = $state([1, 2, 3, 4]);

  function addNumber() {
    numbers[numbers.length] = numbers.length + 1;
  }
  //   $: sum = numbers.reduce((a, b) => a + b, 0);
  let total = $derived(numbers.reduce((a, b) => a + b, 0));

  //   `$:` is not allowed in runes mode, use `$derived` or `$effect` instead
  //   let sum = numbers.reduce((a, b) => a + b, 0);
  //this is not reactive we need to menition either derived or $: before the variable
</script>

<p>{numbers.join(" + ")} = {total}</p>

<button onclick={addNumber}> Add a number </button>
