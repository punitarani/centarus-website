<script>
	import EmailForm from './EmailForm.svelte';

	let innerHeight = 0;
	$: height = innerHeight - 150;
</script>

<svelte:window bind:innerHeight />

<div class="main grid place-items-center" style="height: {height}px;">
	<div class="flex flex-col items-center space-y-2">
		<p class="text-center text-[2.4rem] font-semibold">Coming Soon...</p>
		<EmailForm />
	</div>
</div>

<style>
	.main {
		height: calc(100vh - 150px);
	}
</style>
