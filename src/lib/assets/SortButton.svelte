<div>
	<button> jenicht </button>
</div>

<style>
	div {
		position: relative;
		display: flex;
		align-items: center;
		z-index: 5;
	}

	button {
		position: relative;
		padding: 0.5rem 1rem;
		font-weight: 700;
		text-decoration: none;
		cursor: pointer;
		background: var(--cream-diagonal);
		color: var(--white);
		border-radius: var(--radius-btn);
		border: none;
		text-shadow: 0 0 0.5rem rgba(0 0 0 0.25);
		font-family: var(--font-text);
		font-weight: var(--font-bold);
	}

	button::before,
	button::after {
		content: '';
		position: absolute;
		top: -3px;
		left: -3px;
		width: calc(100% + 6px);
		height: calc(100% + 6px);
		border-radius: var(--radius-btn-border);
	}

	button::before {
		background: var(--silver-horizontal);
		z-index: -1;
	}

	button::after {
		z-index: -2;
		filter: blur(10px);
		opacity: 50%;
		background: var(--cream-horizontal);
	}
</style>
