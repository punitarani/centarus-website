<script>
	export let header;
</script>

<header bind:this={header}>
	<div class="header-container">
		<a href="/">
			<img src="images/logo/centarus-logo-white.png" alt="logo" class="logo" />
		</a>
		<a href="https://github.com/punitarani/centarus-website">
			<img src="images/other/GitHub/github-mark-white.png" alt="GitHub logo" class="github-logo" />
		</a>
	</div>
</header>

<style>
	header {
		height: 100px;

		display: flex;
		justify-content: center;
		align-items: center;
	}

	.header-container {
		height: 60px;
		width: 90%;
		max-width: 1080px;

		box-sizing: border-box;
		padding: 0 24px;

		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	header a {
		height: 100%;

		display: flex;
		align-items: center;
	}

	header .logo {
		height: 90%;
	}

	header .github-logo {
		height: 50%;
	}
</style>
