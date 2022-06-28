<script>
  import { PhoneIcon, MailIcon, LinkedinIcon} from 'svelte-feather-icons';
</script>

<div class="container p-5" id="contact">
  <h1 class="text-center">Contact Our Teams</h1>
  <p class="font-secondary text-center w-80">
    Hubungi kami dengan kontak-kontak dibawah ini 
  </p>

  <div class="row p-5">
    <div class="col px-5">
      <div class="card">
          <img src="https://source.unsplash.com/300x400/?person" class="card-img-top" alt="Blog Media">
          <div class="font-secondary card-body py-4">
            <h2 href="/" class="card-title text-uppercase">
              Pablo J. Bleich 
            </h2>
            <p class="text-center">
              <span class="mx-2">
                <PhoneIcon size={"1x"}/>
              </span>
              <span class="mx-2">
                <MailIcon size={"1x"}/>
              </span>
              <span class="mx-2">
                <LinkedinIcon size={"1x"}/>
              </span>
            </p>
          </div>
      </div>
    </div>
    <div class="col px-5">
      <div class="card">
          <img src="https://source.unsplash.com/300x400/?woman" class="card-img-top" alt="Blog Media">
          <div class="font-secondary card-body py-4">
              <h2 href="/" class="card-title text-uppercase">
                Louise F. Shows 
              </h2>
              <p class="text-center">
                <span class="mx-2">
                  <PhoneIcon size={"1x"}/>
                </span>
                <span class="mx-2">
                  <MailIcon size={"1x"}/>
                </span>
                <span class="mx-2">
                  <LinkedinIcon size={"1x"}/>
                </span>
              </p>
          </div>
      </div>
    </div>
    <div class="col px-5">
      <div class="card">
          <img src="https://source.unsplash.com/300x400/?man" class="card-img-top" alt="Blog Media">
          <div class="font-secondary card-body py-4">
              <h2 href="/" class="card-title text-uppercase">
                Normand Shannon
              </h2>
              <p class="text-center">
                <span class="mx-2">
                  <PhoneIcon size={"1x"}/>
                </span>
                <span class="mx-2">
                  <MailIcon size={"1x"}/>
                </span>
                <span class="mx-2">
                  <LinkedinIcon size={"1x"}/>
                </span>
              </p>
          </div>
      </div>
    </div>
  </div>
</div>

<style>
  .container{
      max-width: none;
      position: relative;
  }

  h1{
      font-size: 4rem;
      color: #064635;
      font-weight: 900;
  }

  h2{
      font-size: 1.2rem;
      font-weight: 800;
      text-align: center;
  }

  .w-80{
      max-width: 80%;
      margin-left: auto;
      margin-right: auto;
  }

  .card{
    border: none;
  }
</style>