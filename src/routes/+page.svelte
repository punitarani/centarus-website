<main>
	<h1 class="title">Centarus</h1>
	<h2 class="tagline">Investing in Humanity</h2>
</main>

<style>
	main {
		height: 100vh;
		width: 100vw;

		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.title {
		font-family: 'Hubot Sans', sans-serif;
		text-align: center;

		font-size: 100px;
		font-weight: 800;
		max-width: 80%;

		margin: 0;
	}

	.tagline {
		font-family: 'Mona Sans', sans-serif;
		text-align: center;
		white-space: nowrap;

		font-size: 42px;
		font-weight: 600;
		max-width: 80%;

		margin: 0;
	}

	@media screen and (max-width: 600px) {
		.title {
			font-size: 60px;
		}

		.tagline {
			font-size: 24px;
		}
	}
</style>
