<script>
	export let classes = '';
	export let size = 'xs';
</script>

<div
	class="container {classes}"
	class:container-xs={size == '' || size == 'xs'}
	class:container-sm={size == 'sm'}
	class:container-md={size == 'md'}
	class:container-lg={size == 'lg'}
	class:container-xl={size == 'xl'}
	class:container-xxl={size == 'xxl'}
>
	<slot />
</div>
