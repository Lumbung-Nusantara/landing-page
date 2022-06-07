<script>
  import Navbar from '../lib/navbar.svelte';
</script>

<main>
  <Navbar />
</main>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  main {
    text-align: center;
    margin: 0 auto;
    background-image: url("/assets/slider1.jpg");
    background-repeat: no-repeat;
    background-size: 100% auto;
    background-position: fixed;
  }
</style>