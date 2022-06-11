<script>
    import { UserIcon, CalendarIcon} from 'svelte-feather-icons';
    import { onMount } from "svelte";

    let blogs = [];
    onMount(async function () {
        const response = await fetch("http://localhost:1337/api/blogs/");
        const res = await response.json();
        blogs = res.data.slice(0,3);
    });
</script>
  
<div class="container bg-green py-5">
    <div class="leaf">
        <img src="assets/leaf3.png" alt="">
    </div>

    <div class="leaf2">
        <img src="assets/leaf4.png" alt="">
    </div>

    <h1 class="text-center text-orange">Lumbung Nusantara Blog</h1>
    <p class="font-secondary text-white text-center w-80">
        Lumbung Nusantara merupakan pioner dari sistem verifikasi dan monitoring supply chain modern berbasis blockchain Cardano yang dapat menjamin keaslian mutu produk organik favorit anda.
    </p>

    <div class="row p-5">
        {#each blogs as blog}
        <div class="col">
            <div class="card">
                <img src="https://source.unsplash.com/1000x600/?vegetables" class="card-img-top" alt="Blog Media">
                <div class="font-secondary card-body py-4">
                    <a href={'http://localhost:3000/blog/' + blog.id} class="card-title text-uppercase">
                        {blog.attributes.title}
                    </a>
                    <hr class="my-4">
                    <div class="row">
                        <div class="col">
                            <span class="fs-smaller">
                                <UserIcon size={"1.2x"}/>
                                Trisha Mediana
                            </span>
                        </div>
                        <div class="col">
                            <span class="fs-smaller">
                                <CalendarIcon size={"1.2x"}/>
                                {blog.attributes.createdAt}
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        {/each}
        <!-- <div class="col">
            <div class="card">
                <img src="https://source.unsplash.com/1500x900/?vegetable" class="card-img-top" alt="Blog Media">
                <div class="font-secondary card-body py-4">
                    <a href="/" class="card-title text-uppercase">
                        Lumbung Nusantara merupakan pioner dari sistem verifikasi
                    </a>
                    <hr class="my-4">
                    <div class="row">
                        <div class="col">
                            <span class="fs-smaller">
                                <UserIcon size={"1.2x"}/>
                                Trisha Mediana
                            </span>
                        </div>
                        <div class="col">
                            <span class="fs-smaller">
                                <CalendarIcon size={"1.2x"}/>
                                9 Juni 2022
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col">
            <div class="card">
                <img src="https://source.unsplash.com/500x300/?fruit" class="card-img-top" alt="Blog Media">
                <div class="font-secondary card-body py-4">
                    <a href="/" class="card-title text-uppercase">
                        Lumbung Nusantara merupakan pioner dari sistem verifikasi
                    </a>
                    <hr class="my-4">
                    <div class="row">
                        <div class="col">
                            <span class="fs-smaller">
                                <UserIcon size={"1.2x"}/>
                                Trisha Mediana
                            </span>
                        </div>
                        <div class="col">
                            <span class="fs-smaller">
                                <CalendarIcon size={"1.2x"}/>
                                9 Juni 2022
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col">
            <div class="card">
                <img src="https://source.unsplash.com/1000x600/?farm" class="card-img-top" alt="Blog Media">
                <div class="font-secondary card-body py-4">
                    <a href="/" class="card-title text-uppercase">
                        Lumbung Nusantara merupakan pioner dari sistem verifikasi
                    </a>
                    <hr class="my-4">
                    <div class="row">
                        <div class="col">
                            <span class="fs-smaller">
                                <UserIcon size={"1.2x"}/>
                                Trisha Mediana
                            </span>
                        </div>
                        <div class="col">
                            <span class="fs-smaller">
                                <CalendarIcon size={"1.2x"}/>
                                9 Juni 2022
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div> -->
    </div>
</div>

<style>

    .container{
        max-width: none;
        position: relative;
    }

    .leaf{
        position: absolute;
        left: 20px;
        top: 0;
        animation: up-down infinite 4s linear;
    }

    .leaf2{
        position: absolute;
        right: 90px;
        top: 0;
        animation: up-down infinite 4s linear;
    }

    h1{
        font-size: 4rem;
        color: white;
        font-weight: 900;
    }

    .w-80{
        max-width: 80%;
        margin-left: auto;
        margin-right: auto;
    }

    .text-orange{
        color: #FAB522;
    }

    a{
        text-decoration: none;
        color: black;
    }

    a:hover{
        color: #519259;
    }

    .card-title{
        font-size: 1.4rem;
        line-height: 1.4;
        font-weight: 600;
    }

    .card{
        box-shadow: rgba(0, 0, 0, 0.3) 0px 19px 38px, rgba(0, 0, 0, 0.22) 0px 15px 12px;
    }

    @keyframes up-down{
        0% {
        -webkit-transform: translateY(-20px);
        transform: translateY(-20px);
        }
        50% {
            -webkit-transform: translateY(-10px);
            transform: translateY(-10px);
        }
        100% {
            -webkit-transform: translateY(-20px);
            transform: translateY(-20px);
        }
    }
    
</style>