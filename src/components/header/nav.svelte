<script>
	import NavBar from './navBar.svelte';
	import NavMenu from './navMenu.svelte';
</script>

<!--Computer Nav Bar-->
<div class="hidden lg:block">
	<NavBar />
</div>

<!--Mobile Nav Menu-->
<div class="visible lg:hidden">
	<NavMenu />
</div>
