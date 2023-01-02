<script>
	import Logo from '/src/components/logo.svelte';
	import Nav from './nav.svelte';
</script>

<header class="mt-2 flex h-20 items-center justify-center">
	<div class="flex h-16 w-10/12 max-w-screen-xl flex-row items-center justify-between">
		<a href="/">
			<Logo size="text-4xl" />
		</a>
		<Nav />
	</div>
</header>
