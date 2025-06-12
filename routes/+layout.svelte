<script lang="ts">
	import '../app.css';
	import Nav from './Components/Nav.svelte';
	import Footer from "./Components/footer.svelte";
	let { children } = $props();
</script>
<head>
	<link
	rel="stylesheet"
	href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
	integrity="sha512-..."
	crossorigin="anonymous"
	referrerpolicy="no-referrer"
  />
  	<title>Asafesseidon's Website</title>

  </head>
<Nav />
{@render children()}

<Footer />

