<script>
	export let type;
</script>

<div class="wrapper">
	<span class={type}>  <slot />  </span>
</div>



<style>

	span {
			color: white;
			width: auto;
			/* padding-top: 3rem;
			padding-bottom: 3rem; */
			padding-right: 0.3rem;
			padding-left: 0.3rem;
			border: 0;
			border-radius: 2rem;
			font-weight: 400;
			/* display: grid;
			justify-content: center;
			align-items: baseline; */
	}


	.default {
			background-color: var(--default-color);
		}

	.primary {
			background-color: var(--primary-color);
		}

	.secondary {
			background-color: var(--secondary-color);
		}

	.accent {
		background-color: var(--accent-color);
	}

	.ghost {
		background-color: var(--ghost-color);
		color: var(--secondary-font-color);
		border: 1px solid;
	}




</style>