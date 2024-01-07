<script>
	export let classes = '';
	export let color = 'success';
</script>

<div
	class="{classes}"
	class:primary={color === 'primary'}
	class:secondary={color === 'secondary'}
	class:tertiary={color === 'tertiary'}
	class:success={color === 'success'}
	class:danger={color === 'danger'}
	class:warning={color === 'warning'}
	class:info={color === 'info'}
	class:light={color === 'light'}
	class:dark={color === 'dark'}
>
	<slot />
</div>

<style>
	div {
		display: inline-block;
		align-content: center;
		line-height: 16px;
		font-size: 12px;
		font-weight: bold;
		border-radius: .25rem;
		padding: .15rem .3rem;
	}

	.light {
		background-color: var(--light);
		color: var(--text);
	}

	.dark {
		background-color: var(--dark);
		color: var(--text-light);
	}

	.primary {
		background-color: var(--primary);
		color: var(--text-light);
	}

	.secondary {
		background-color: var(--secondary);
		color: var(--text);
	}

	.tertiary {
		background-color: var(--tertiary);
		color: var(--text);
	}

	.success {
		background-color: var(--success);
		color: var(--text-light);
	}

	.danger {
		background-color: var(--danger);
		color: var(--text-light);
	}

	.warning {
		background-color: var(--warning);
		color: var(--text);
	}

	.info {
		background-color: var(--info);
		color: var(--text);
	}
</style>
