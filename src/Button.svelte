<script>
	export let type;
	export let mode;
</script>

<button class:inversed={mode === "inversed"} class={type}>  <slot /> </button>

<style>

	/* GENERAL */
	button {
		color: white;
		transition: all 0.3s;
		width: auto;
		padding: 0.7rem;
		border-radius: 0.5rem;
		border: 0;
		font-weight: 600;
		text-transform: uppercase;
		font-size: 0.7rem;
	}


	/* DEFAULT */
	.default {
		background-color: var(--default-color);
	}

	.default:hover {
		background-color:hsl(219,14%,38%);
	}


	/* PRIMARY  */
	.primary {
		background-color: var(--primary-color);
	}

	.primary:hover {
		background-color: green;
	}

	.primary.inversed {
		background-color: red;
	}


	/* SECONDARY */
	.secondary {
		 background-color: var(--secondary-color);
	}

	.secondary:hover {
		background-color: green;
	}

	.secondary.inversed {
		background-color: yellow;
	}

	/* ACCENT  */
	.accent {
		background-color: var(--accent-color);
	}

	.accent:hover {
		background-color: green;
	}

	.accent.inversed {
		background-color: red;
	}

	/* GHOST  */
	.ghost {
		background-color: transparent;
		color: var(--secondary-font-color);
	}

	.ghost:hover {
		background-color: green;
	}

	.ghost.inversed {
		background-color: red;
	}

	/* LINK  */
	.link {
		background-color: transparent;
		color: var(--link-font-color);
	}

	.link:hover {
		background-color: green;
	}

	.link.inversed {
		background-color: red;
	}


</style>