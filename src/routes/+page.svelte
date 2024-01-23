<script>
  import { goto } from '$app/navigation'
	import logo from '../img/fg-logo.png';
  import Footer from '$lib/components/Footer.svelte'
	import './global.css';
  const handleBusinessClick = () => {
      goto('/business')
  }
  const handleMarineClick = () => {
      goto('/marine')
  }
</script>

<main>
	<div class="grid-container">
		<div class="top">
			<img src={logo} alt="logo" />
		</div>
		<div class="business">
			<h1>Business services</h1>
			<p>
				LAb consequuntur cumque distinctio excepturi fuga iure laudantium molestias quidem ratione
				saepe sint, tempore temporibus tenetur ullam!
			</p>
			<button on:click={handleBusinessClick}>Business</button>
		</div>
		<div class="marine">
			<h1>Marine services</h1>
			<p>
				Ab consequuntur cumque distinctio excepturi fuga iure laudantium molestias quidem ratione
				saepe sint, tempore temporibus tenetur ullam!
			</p>
			<button on:click={handleMarineClick}>Marine</button>
		</div>
	</div>

  <Footer/>
</main>

<style>
	main {
		background-color: #010101;
	}

	.top img {
		/*border: white 3px solid;*/
		width: 100%;
		/*margin: auto;*/
	}

	.top {
		border-radius: 8px;
		grid-column: span 2;
		background-color: rgba(255, 255, 255, 0.6);
		/*place-content: center;*/
		margin: 20px;
		display: flex;
		justify-content: center;
	}

	.grid-container {
		display: grid;
		justify-content: space-evenly;
		grid-template-columns: 1fr 1fr;
		background-color: rgba(255, 255, 255, 0.5);
		background-image: url('../img/fire-background1024w.jpg');
		background-color: #cccccc;
		background-size: cover;
		background-position: center center;
		max-width: 700px;
		margin: 0 auto;
	}

	.business,
	.marine {
		/*border: white solid 5px;*/
		border-radius: 8px;

		background: rgba(255, 255, 255, 0.6);

		margin: 0 20px 20px 20px;
		padding: 0 20px 20px 20px;
		line-height: 1.8em;
	}

	h1 {
		color: #000;
		font-size: 2.6em;
		line-height: 1em;
	}

	p {
		color: #000000;
		font-size: 1.2em;
	}

	button {
		display: block;
		box-sizing: border-box;
		margin: 0 auto;
		padding: 8px;
		width: auto;
		max-width: 200px;
		background: rgba(255, 255, 255, 0.5);
		border-radius: 8px;
		/*color: #000;*/
		text-align: center;
		text-decoration: none;
		letter-spacing: 1px;
		transition: all 0.3s ease-out;
		border: 3px white solid;
		font-size: 2.6em;
	}

	h1 {
		text-align: center;
	}
</style>
