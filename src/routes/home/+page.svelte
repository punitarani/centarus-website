<script>
	import { onMount } from 'svelte';
	import EmailForm from './EmailForm.svelte';

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

<div class="main grid place-items-center" bind:this={main}>
	<div class="flex flex-col items-center space-y-2">
		<p class="text-[2.4rem] text-center">Coming Soon...</p>
		<EmailForm />
	</div>
</div>

<style>
	.main {
		height: calc(100vh - 100px - 50px - 20px);
	}
</style>
