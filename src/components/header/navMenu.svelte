<script>
	const MenuItems = {
		Home: '/home',
		Mission: '/mission'
	};

	let menuOpen = 'hidden'; // Menu state (hidden (default) or visible)

	// Open/Close the menu when the menu button is clicked
	function menuHandler() {
		if (menuOpen === 'hidden') {
			menuOpen = 'visible';
		} else {
			menuOpen = 'hidden';
		}
	}
</script>

<div class="relative">
	<button class="align-center flex" on:click={menuHandler}>
		<span class="material-symbols-rounded">menu</span>
	</button>

	<div class="absolute right-1 z-10">
		<nav class="mt-2 text-right {menuOpen}">
			<ul class="flex flex-col">
				{#each Object.keys(MenuItems) as item}
					<li class="mt-1">
						<a href={MenuItems[item]} class="text-lg">{item}</a>
					</li>
				{/each}
			</ul>
		</nav>
	</div>
</div>

<style>
	.material-symbols-rounded {
		font-size: 32px;
	}
</style>
