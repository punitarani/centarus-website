<script>
	import { onMount } from 'svelte';

	// main div
	let main;

	// onMount is a lifecycle hook that runs after the component is mounted
	onMount(() => {
		// Height of the browser viewport
		const height = window.innerHeight;

		// Set the height of the container to the height of the browser minus header and footer
		// 	Also account for the padding on the main element
		// This ensures that the footer is always at the bottom of the page
		const mainHeight = height - 100 - 50 - 20;
		main.style.height = `${mainHeight}px`;
	});
</script>

<div class="main" bind:this={main}>
	<p>Coming Soon...</p>
</div>

<style>
	.main {
		height: calc(100vh - 100px - 50px - 20px);

		display: flex;
		justify-content: center;
		align-items: center;
	}

	.main p {
		font-size: 2rem;
	}
</style>
