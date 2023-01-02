<script>
	const MenuItems = {
		Home: '/home',
		Mission: '/mission'
	};
</script>

<nav>
	<ul class="flex">
		{#each Object.keys(MenuItems) as item}
			<li class="mx-6">
				<a href={MenuItems[item]}>{item}</a>
			</li>
		{/each}
	</ul>
</nav>
