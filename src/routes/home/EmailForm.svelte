<script lang="ts">
	let email = '';
	let errorMessage = '';
	let submitSuccess = false;

	// validateEmail validates the email address
	function validateEmail(email) {
		const emailRegEx =
			/^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
		return emailRegEx.test(String(email).toLowerCase());
	}

	// submitEmail handles the form submission
	function submitEmail() {
		if (email.length == 0) {
			errorMessage = 'Please enter an email address';
		} else if (!validateEmail(email)) {
			errorMessage = 'Please enter a valid email address';
		} else {
			errorMessage = '';
		}

		console.log(email);
		console.log(errorMessage);

		// If there are no errors, submit the email
		if (errorMessage.length == 0) {
			submitSuccess = true;
		}
	}
</script>

{#if !submitSuccess}
	<form class="flex flex-row">
		<input
			type="email"
			placeholder="Email Address"
			class="w-48 bg-slate-100 text-black"
			bind:value={email}
		/>
		<button
			class="flex inline-flex w-16 flex-row items-center justify-center bg-green-700 text-slate-100"
			on:click={submitEmail}
			>Submit
		</button>
	</form>
{:else}
	<div class="h-8 text-slate-100">
		<p>Thank you for your interest!</p>
	</div>
{/if}

<style>
	form input,
	form button {
		font-family: 'Mona Sans', sans-serif;
		font-size: 0.75rem;

		height: 30px;
		border: 0;
		margin: 0 0.25rem;
		padding: 0 1rem;
		border-radius: 12px;
	}
</style>
