<script>
	import Badge from "./Badge.svelte"
	import Button from "./Button.svelte"
</script>

<article>
	<img src="imgs/nice_shoe.webp" alt="">

	<div class="card_content_wrapper">
		<div class="card_titel">
			<h3>Shoes!</h3>
			<Badge type ="secondary"> NEW </Badge>
		</div>
	
		<div>
			<p>if a dog chews shoes whose shoes does he choose?</p>

			<div class="badges">
				<Badge type ="ghost"> Fashion </Badge>
				<Badge type ="ghost"> Product </Badge>
			</div>
		</div>

		<div class="button">
			<Button type ="primary"> BUY NOW </Button>
		</div>
	</div>
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

.card_titel {
	display: flex;
	align-items: center;
	gap: 0.5rem;
}

.card_content_wrapper {
	padding: 1rem;
	grid-row: 2/3;
}

.badges {
	display: flex;
	gap: 0.5rem;
	font-size: 0.7rem;
}


.button {
	position: relative;
	float: right;
}

h3 {
	margin: 0px;
}

img {
	grid-row: 1/2;
	border-top-right-radius: 1rem;
	border-top-left-radius: 1rem;
	width: 100%;
	height: 100%;
	object-fit: cover;
}

p {
	font-size: 0.7rem;
}






</style>