<script>
  import './style.css';
  import { Router, Route } from "svelte-routing";
  import Landing from "./page/landing.svelte";
  import Blogs from "./page/blogs.svelte";
  import Blog from "./page/blog.svelte";
  
	export let url= "";
</script>

<body>
  <Router {url}>
    <Route path="/" component={Landing} />
    <Route path="blogs" component={Blogs} />
    <!-- <Route path="blog:id" component={Blog} /> -->
    <Route path="blog" component={Blog} />
  </Router>
</body>
