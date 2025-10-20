/<!-- logic -->
<script lang="ts">
  let title:string = "svelte";
</script>

<!-- markup -->
<h1>
  hello {title as string}
</h1>

<!-- styles -->
<style>
  h1 {
    color: orangered;
  }
</style>
