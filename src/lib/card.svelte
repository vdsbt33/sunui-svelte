<script>
	export let classes = '';
</script>

<div class="{classes}">
	<slot />
</div>

<style>
	div {
		padding: .75rem;
		display: block;
		background-color: var(--light);
		border-radius: 1rem;
		box-shadow: 0 0 4px #00000015;
	}
</style>

