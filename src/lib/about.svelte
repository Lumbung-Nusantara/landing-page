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
      background-image: url("/assets/bg15.jpg");
      background-repeat: no-repeat;
      background-size: 100% auto;
      background-position: fixed;
    }
  
    img {
      height: 16rem;
      width: 16rem;
    }

  
    p {
      max-width: 14rem;
      margin: 1rem auto;
      line-height: 1.35;
    }
  
    @media (min-width: 480px) {
      h1 {
        max-width: none;
      }
  
      p {
        max-width: none;
      }
    }
  </style>