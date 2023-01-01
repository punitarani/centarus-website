<script>
	export let header;
</script>

<header class="mt-4 flex h-20 items-center justify-center" bind:this={header}>
	<div class="header-container flex h-16 w-10/12 max-w-screen-xl flex-row justify-between">
		<a href="/">
			<img src="images/logo/centarus-logo-white.png" alt="logo" class="h-16" />
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
