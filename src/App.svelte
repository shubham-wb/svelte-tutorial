<!-- logic -->
<script lang="ts">
  const obj = {
    src: "https://media.cnn.com/api/v1/images/stellar/prod/211227135008-02-the-batman-trailer.jpg?c=16x9&q=h_653,w_1160,c_fill/f_avif",
    alt: "The Batman Movie Poster",
  };
  const lazy = false;
</script>

/<!-- markup -->
<img src={obj.src} alt={obj.alt} loading={lazy ? "lazy" : null} />

<!-- styles -->
