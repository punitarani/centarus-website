<script>
	import Logo from '/src/components/logo.svelte';
</script>

<header class="mt-4 flex h-20 items-center justify-center">
	<div class="header-container flex h-16 w-10/12 max-w-screen-xl flex-row justify-between">
		<a href="/">
			<Logo size="text-4xl" />
		</a>
		<a href="https://github.com/punitarani/centarus-website">
			<img src="images/other/GitHub/github-mark-white.png" alt="GitHub logo" class="h-8" />
		</a>
	</div>
</header>

<style>
	header a {
		display: flex;
		align-items: center;
	}
</style>
