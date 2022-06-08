<script>
    import Navbar from './navbar.svelte';
</script>

<div class="bg-hero pb-5">
    <Navbar />
    <div class="container py-5">
        <div class="row">
          <div class="col-8 align-self-center">
            <h1 class="text-start">Organik tidak harus mahal.</h1>
          </div>
        </div>
        <div class="row">
          <div class="col-6">
            <p class="font-secondary text-start">
             Dapatkan jaminan kualitas makanan organik terpercaya dengan verifikasi oleh teknologi blockchain Cardano.
            </p>

            <button type="button" class="btn btn-hero fw-bolder fs-smaller my-4">LEARN MORE</button>
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

    .btn-hero{
        color: white;
        background-color: #064635;
        padding: 1rem 2rem;
        border-radius: 0 2rem 2rem 2rem;
        float: left;
    }
</style>