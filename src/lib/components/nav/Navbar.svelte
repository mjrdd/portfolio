<script lang="ts">
	import NavbarItem from "./NavbarItem.svelte";
	import NavbarList from "./NavbarList.svelte";

	export let title = "";
</script>

<nav class="navbar" aria-label="primary">
	<div class="nav">
		<div class="nav-brand">
			<span>{title}</span>
		</div>
		<NavbarList>
			<NavbarItem href="/" label="Home" />
			<NavbarItem href="/aboutme" label="About Me" />
		</NavbarList>
	</div>
</nav>

<style lang="postcss">
	.navbar {
		width: 100%;
		height: 56px;
		user-select: none;
	}

	.nav {
		width: min(95%, 1280px);
		height: 100%;
		margin: 0 auto;
		display: flex;
		justify-content: space-between;
	}

	.nav-brand {
		display: flex;
		align-items: center;
		justify-content: center;
	}
</style>
