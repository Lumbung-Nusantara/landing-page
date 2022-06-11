<script>
  import Navbar from '../lib/navbar.svelte';
  import BlogContent from '../lib/blog-content.svelte';
  import Footer from '../lib/footer.svelte';

  export let id;
  console.log(id)
</script>

<main>
  <Navbar />
  <BlogContent id={id}/>
  <Footer />
</main>