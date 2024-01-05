<script>
	export let classes = '';
	export let color = 'primary';
	export let grow = true;
</script>

<button
	type="button"
	on:click
	class={classes}
	class:primary={color === 'primary'}
	class:secondary={color === 'secondary'}
	class:tertiary={color === 'tertiary'}
	class:danger={color === 'danger'}
	class:warning={color === 'warning'}
	class:w-100={grow === true}
>
	<slot>
		Button
	</slot>
</button>

<style>
	button {
		font-size: 14px;
		font-weight: 500;
		border: none;
		border-radius: .25rem;
		padding: .5rem .75rem;
		cursor: pointer;
		user-select: none;
	}

	.primary {
		background-color: var(--primary);
		color: var(--text);
	}
	.primary:hover {
		background-color: var(--primary-dark);
	}

	.secondary {
		background-color: var(--secondary);
		color: var(--text);
	}
	.secondary:hover {
		background-color: var(--secondary-dark);
	}

	.tertiary {
		background-color: var(--tertiary);
		color: var(--text);
	}
	.tertiary:hover {
		background-color: var(--tertiary-dark);
	}

	.danger {
		background-color: var(--danger);
		color: var(--text-dark);
	}
	.danger:hover {
		background-color: var(--danger-dark);
	}

	.warning {
		background-color: var(--warning);
		color: var(--text);
	}
	.warning:hover {
		background-color: var(--warning-dark);
	}

</style>
