<script>
    
</script>

<section class="bg-bc">
  <div class="bc py-5">
    <div class="py-5 my-5">
      <h1 class="text-center text-white">Blogs</h1>
      <p class="font-secondary text-white text-center">
        HOME > BLOGS
      </p>
    </div>
  </div>
</section>

<style>
    h1 {
        font-size: 6rem;
        font-weight: 900;
        line-height: 1.2;
        z-index: 100;
    }

    p {
        margin: 0rem 0;
        letter-spacing: 1px;
        line-height: 1.35;
    }

    .bc{
      position: relative;
    }

    .bg-bc{
        position: relative;
        margin: 0 auto;
        background-image: url("https://images.pexels.com/photos/6489734/pexels-photo-6489734.jpeg");
        background-size: 100% auto;
    }

    .bg-bc::before{
      content: "";
      background-color: #000;
      opacity: 0.5;
      position: absolute;
      left: 0;
      width: 100%;
      height: 100%;
    }
</style>