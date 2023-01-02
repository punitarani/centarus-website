<script>
	import '/src/app.css';
	import Header from '/src/components/header/header.svelte';
	import Footer from '/src/components/footer/footer.svelte';
</script>

<Header />
<slot />
<Footer />
