<script>
    import Navbar from './navbar.svelte';
</script>

<div class="bg-hero pb-5">
    <Navbar />
    <div class="container py-4">
        <div class="row mt-5">
          <div class="col-8 align-self-center">
            <h1 class="text-start">Organic Food is Good for Health</h1>
          </div>
        </div>
        <div class="row mb-5">
          <div class="col-6 align-self-start">
            <p class="font-secondary text-start">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
              sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </p>
          </div>
        </div>
    </div>
</div>

<style>
    h1 {
        font-size: 6rem;
        font-weight: 500;
        line-height: 1.4;
    }

    p {
        margin: 0rem 0;
        letter-spacing: 1px;
        line-height: 1.35;
    }

    .bg-hero{
        text-align: center;
        margin: 0 auto;
        background-image: url("/assets/slider1.jpg");
        background-repeat: no-repeat;
        background-size: 110% auto;
        background-position: fixed;
    }
</style>