<script>
	import Badge from "./Badge.svelte"
	import Button from "./Button.svelte"
	import Footer from "./Footer.svelte"
	import Card from "./Card.svelte"
	import Button_w_badge from "./Button_w_badge.svelte"
	import Avatar_w_indicator from "./Avatar_w_indicator.svelte"
</script>








<body>

	<h1>Opgave : Design System => Kode</h1>
	

	<!-- FOOTER -->
	<section>
		<h2>A. Footer component</h2>
		<Footer />

		<div class="documentation_container">

			<h3>Documentation</h3>

			<div >
				

			</div>
		</div>

	</section>


	<!-- BADGES -->
	<section>
		<h2>B. Badge component</h2>
		<div class="badge_wrapper">
			<Badge type ="default"> Default </Badge>
			<Badge type ="primary"> Primary </Badge>
			<Badge type ="secondary"> Secondary </Badge>
			<Badge type ="accent"> Accent </Badge>
			<Badge type ="ghost"> Ghost </Badge>
		</div>

		<div class="documentation_container">

			<h3>Documentation</h3>

			<div class="documentation">
				<pre> <code>{'<span class={types}>  <slot />  </span> '} </code></pre>
			</div>
		</div>


	</section>


	<!-- BUTTONS -->
	<section>
		<h2>C. Button component</h2>
		<div class="button_wrapper">
			
			<Button type ="default"> Default </Button>
			<!-- <Button type ="default" mode="inversed"> Default Inversed </Button> -->

			<Button type ="primary"> Primary </Button>
			<!-- <Button type ="primary" mode="inversed"> Primary Inversed </Button> -->

			<Button type ="secondary"> Secondary </Button>
			<!-- <Button type ="secondary" mode="inversed"> Secondary Inversed </Button> -->

			<Button type ="accent"> Accent </Button>
			<!-- <Button type ="accent" mode="inversed"> Accent Inversed </Button> -->

			<Button type ="ghost"> Ghost </Button>
			<!-- <Button type ="ghost" mode="inversed"> Ghost Inversed </Button> -->

			<Button type ="link"> Link </Button>
			<!-- <Button type ="link" mode="inversed"> Link Inversed </Button> -->
		</div>

		<div class="documentation_container">

			<h3>Documentation</h3>

			<div class="documentation">
				<pre> <code>{'<button class:inversed={mode === "inversed"} class={type}>  <slot /> </button>'} </code></pre>
			</div>
		</div>
	</section>


	<!-- CARD -->
	<section>
		<h2>D. Card component</h2>
		<div class="card_wrapper">
			<Card />
		</div>

		<div class="documentation_container">

			<h3>Documentation</h3>

			<div class="documentation">
				<pre> <code>{'<button class:inversed={mode === "inversed"} class={type}>  <slot /> </button>'} </code></pre>
			</div>
		</div>
	</section>

	<!-- BUTTON WITH BADGE -->
	<h2>E. Button w. badge component</h2>
	<section>
		<div class="button_w_badge_wrapper">
				<Button_w_badge type ="default"> Inbox </Button_w_badge>
		</div>

		<div class="documentation_container">

			<h3>Documentation</h3>

			<div class="documentation">
				<pre> <code>{'<button class:inversed={mode === "inversed"} class={type}>  <slot /> </button>'} </code></pre>
			</div>
		</div>
	</section>

		<!-- AVATAR WITH INDICATOR -->
	<section>
		<h2>A.Avatar w. indicator component</h2>
		<div class="avatar_container">
			<Avatar_w_indicator size="XL"> K </Avatar_w_indicator>
			<Avatar_w_indicator size="large" mode="online"> JO </Avatar_w_indicator>
			<Avatar_w_indicator size="medium"> MX </Avatar_w_indicator>
			<Avatar_w_indicator size="small"> AA </Avatar_w_indicator>
		</div>

		<div class="documentation_container">

			<h3>Documentation</h3>

			<div class="documentation">
				<pre> <code>{'<button class:inversed={mode === "inversed"} class={type}>  <slot /> </button>'} </code></pre>
			</div>
		</div>
	</section>
</body>


<style>

	.badge_wrapper {
		display: flex;
		gap: 1rem;
		justify-content: center;
	}

	.button_wrapper {
		display: flex;
		gap: 1rem;
		justify-content: center;
	}

	.card_wrapper {
		display: flex;
		gap: 1rem;
		justify-content: center;
	}

	.button_w_badge_wrapper {
		display: flex;
		gap: 1rem;
		justify-content: center;
	}

	.avatar_container {
		display: flex;
		gap: 1rem;
		justify-content: center;
	}

</style>