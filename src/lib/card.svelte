<script>
	export let classes = '';
</script>

<div class="p-3 {classes}">
	<slot />
</div>

<style>
	div {
		display: inline-block;
		background-color: var(--light);
		border-radius: 1rem;
		box-shadow: 0 0 3px #00000011;
	}
</style>
