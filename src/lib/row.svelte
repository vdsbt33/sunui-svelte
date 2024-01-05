<script>
	export let gap = 1;
</script>

<div
	class="row grid-gap-{gap}"
>
	<slot />
</div>

<style>
	div {
		display: grid;
	}
</style>


