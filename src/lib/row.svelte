<script>
	export let justify = 'start';
	export let classes = '';
</script>

<div
	class="row justify-content-{justify} {classes}"
>
	<slot />
</div>

