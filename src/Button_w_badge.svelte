<script>
	import Badge from "./Badge.svelte"
	import Button from "./Button.svelte"
	export let type;
	export let mode;
</script>

<div class="container">
	<div class="badge">
		<Badge type ="secondary"> 99+ </Badge>
	</div>
	
	<Button type ="default"> INBOX </Button>
</div>


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
		background-color: red;
	}

	.secondary {
			background-color: var(--secondary-color);
		}

	.badge {
		position: relative;
		left: 40px;
		top: 7px;
		font-size: 0.8rem;
	}



	


</style>