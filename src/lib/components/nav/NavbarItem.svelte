<script lang="ts">
	export let href = "/";
	export let label = "";
</script>

<a class="nav-item" {href}>{label}</a>

<style lang="postcss">
	.nav-item {
		padding: 0 16px;
		display: flex;
		align-items: center;
		justify-content: center;
		cursor: pointer;
		color: inherit;
		text-decoration: none;

		&:hover {
			background-color: rgba(0, 0, 0, 0.1);
		}
	}
</style>
