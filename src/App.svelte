<script>
  let string = `this string contains some <strong>HTML!!!</strong>`;
  import Nested from "./nested.svelte";
</script>

<p>This is a paragraph.</p>
<Nested />
<!-- using custom components  -->
{@html string}

<!-- render the HTML string -->
<style>
  p {
    color: goldenrod;
    font-family: "Comic Sans MS", cursive;
    font-size: 2em;
  }
</style>
