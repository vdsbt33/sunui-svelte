<script>
	export let variant = 'p';
	export let size    = 14;
	export let weight  = 400;
	export let italic  = false;
	export let bold    = false;
	export let classes = '';
</script>

{#if variant === 'p'}
	<p
		class="font-weight-{weight} {classes}"
		class:text-bold={bold}
		class:text-italic={italic}
	>
		<slot />
	</p>
{:else if variant === 'h5'}
	<h5
		class="font-weight-{weight} {classes}"
		class:text-bold={bold}
		class:text-italic={italic}
	>
		<slot />
	</h5>
{:else if variant === 'h4'}
	<h4
		class="font-weight-{weight} {classes}"
		class:text-bold={bold}
		class:text-italic={italic}
	>
		<slot />
	</h4>
{:else if variant === 'h3'}
	<h3
		class="font-weight-{weight} {classes}"
		class:text-bold={bold}
		class:text-italic={italic}
	>
		<slot />
	</h3>
{:else if variant === 'h2'}
	<h2
		class="font-weight-{weight} {classes}"
		class:text-bold={bold}
		class:text-italic={italic}
	>
		<slot />
	</h2>
{:else if variant === 'h1'}
	<h1
		class="font-weight-{weight} {classes}"
		class:text-bold={bold}
		class:text-italic={italic}
	>
		<slot />
	</h1>
{/if}

