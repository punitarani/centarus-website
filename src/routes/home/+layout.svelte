<script>
	import '/src/global.css';
	import Header from '/src/components/header/Header.svelte';
	import Footer from '/src/components/footer/Footer.svelte';
</script>

<Header />
<slot />
<Footer />
