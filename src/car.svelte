<script>
	export let model;
	export let make;
	export let price;
</script>

<article>
	<h2>
		{model} - {make}
	</h2>

	<p>
		Nu kun  {price}
	</p>
</article>



<style>

article{
	width: 325px;
	height: 350px;
	border-radius: 1rem;
	display: grid;
	grid-template-rows: 60% 40%;
	box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}



</style>