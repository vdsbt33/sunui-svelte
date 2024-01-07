<script>
	export let justify = 'start';
	export let align = 'center';
	export let classes = '';
</script>

<div
	class="row justify-content-{justify} align-items-{align} {classes}"
>
	<slot />
</div>

