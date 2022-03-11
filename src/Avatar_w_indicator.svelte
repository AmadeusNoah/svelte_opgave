<script>
	export let mode;
	export let size;
</script>


<section class={size}>
	<div class={mode}> </div>
	<p> <slot /> </p> 
</section>





<style>

	section {
			color: white;
			width: auto;
			height: 100px;
			width: 100px;
			background-color: var(--default-color);
			border: 0;
			border-radius: 50%;
			display: flex;
			justify-content: center;
			align-items: center;
			position: relative;
	}


	.online {
		width: 20%;
		height: 20%;
		position: absolute;
		background-color: green;
		border-radius: 50%;
		border: 2px solid white;
		top: 1%;
		right: 5%;
		}

	.small {
		height: 2rem;
		width: 2rem;
	}

	.medium {
		height: 3rem;
		width: 3rem;
	}

	.large {
		height: 4rem;
		width: 4rem;
	}

	.xl {
		height: 5rem;
		width: 5rem;
	}







</style>