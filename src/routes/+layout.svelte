<script>
	// Stying
	import '@fontsource-variable/space-grotesk';
	import '$lib/styles/global.css';
	//

	import NavBar from '$lib/components/NavBar.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<NavBar />
<slot />
<Footer />
