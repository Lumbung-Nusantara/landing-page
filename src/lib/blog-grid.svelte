<script>
    import { UserIcon, CalendarIcon} from 'svelte-feather-icons';
    import { onMount } from "svelte";

    let blogs = [];
    onMount(async function () {
        const response = await fetch("http://localhost:1337/api/blogs/");
        const res = await response.json();
        blogs = res.data;
    });
</script>
  
<div class="container py-5">
    <div class="row p-5">
        {#each blogs as blog}
        <div class="col-4">
            <div class="card">
                <img src="https://source.unsplash.com/1500x900/?vegetables" class="card-img-top" alt="Blog Media">
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
        <!-- <div class="col-4">
            <div class="card">
                <img src="https://source.unsplash.com/1500x900/?vegetables" class="card-img-top" alt="Blog Media">
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
        <!-- <div class="col-4">
            <div class="card">
                <img src="https://source.unsplash.com/500x300/?fruits" class="card-img-top" alt="Blog Media">
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
        <!-- <div class="col-4">
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
        box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
    }
    
</style>