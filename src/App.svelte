<script>
  import './style.css';
  import { Router, Route } from "svelte-routing";
  import Landing from "./page/landing.svelte";

	export let url= "";
</script>

<body>
  <Router {url}>
    <Route path="/" component={Landing} />
  </Router>
</body>