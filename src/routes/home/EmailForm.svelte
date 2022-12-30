<script lang="ts">
	let email = '';

	// submitEmail handles the form submission
	function submitEmail() {
		console.log(email);
	}
</script>

<form class="form-sign-up">
	<input type="email" placeholder="Email Address" class="input-email" bind:value={email} />
	<button class="button-email-submit" on:click={submitEmail}>Submit</button>
</form>

<style>
	form {
		display: flex;
		flex-direction: row;
	}

	form input,
	form button {
		font-family: 'Mona Sans', sans-serif;
		font-size: 0.75rem;

		height: 30px;
		border: 0;
		margin: 0 0.25rem;
		padding: 0 1rem;
		border-radius: 12px;

		display: inline-flex;
		align-items: center;
	}

	form input {
		width: 150px;
		justify-content: flex-start;

		background-color: #e6e6e6;
	}

	form button {
		width: 70px;
		justify-content: center;

		color: #e6e6e6;
		background-color: green;
	}
</style>
