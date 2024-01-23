<script>
  import Footer from '$lib/components/Footer.svelte';
  // import '../app.postcss';
</script>

<main>
  <div class="container">
    <slot />
    <Footer />
  </div>
</main>

<style>
    *, *::before, *::after {
        box-sizing: border-box;
    }

    main {
        /*max-width: 1200px;*/
        margin: 0 auto;
        width: 80%;
    }

    :global(html) {
        overflow-y: scroll;
        /*background: #F8F0E3;*/
        font-family: 'Golos Text', sans-serif;
    }

</style>