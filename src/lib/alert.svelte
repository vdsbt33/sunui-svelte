<script>
	export let classes = '';
	export let color = 'success';
	export let visible = true;

	function hide() {
		visible = false;
	}
</script>

<div
	class="{classes}"
	class:hide={!visible}
	class:primary={color === 'primary'}
	class:secondary={color === 'secondary'}
	class:tertiary={color === 'tertiary'}
	class:success={color === 'success'}
	class:danger={color === 'danger'}
	class:warning={color === 'warning'}
	class:info={color === 'info'}
>
	<slot />
	<button on:click={hide}>&#10799;</button>
</div>

<style>
	div {
		padding: .5rem 0.75rem;
		border-radius: .25rem;
		margin: .0 .25rem .5rem .25rem;
		display: flex;
		justify-content: space-between;
	}
	button {
		border: none;
		margin: 0;
		padding: 0;
		background-color: transparent;
		user-select: none;
		cursor: pointer;
		font-size: 16px;
		width: 16px;
		height: 16px;
		line-height: 18px;
	}

	.hide {
		display: none;
	}

	.primary {
		background-color: var(--primary);
		border: 1px solid var(--primary-border);
	}

	.secondary {
		background-color: var(--secondary);
		border: 1px solid var(--secondary-border);
	}

	.tertiary {
		background-color: var(--tertiary);
		border: 1px solid var(--tertiary-border);
	}

	.success {
		background-color: var(--success);
		border: 1px solid var(--success-border);
	}

	.danger {
		background-color: var(--danger);
		border: 1px solid var(--danger-border);
	}

	.warning {
		background-color: var(--warning);
		border: 1px solid var(--warning-border);
	}

	.info {
		background-color: var(--info);
		border: 1px solid var(--info-border);
	}
</style>
