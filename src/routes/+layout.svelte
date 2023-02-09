<script>
	import Header from './Header.svelte';
	import './styles.css';

	/*

			<Header />


	<footer>
		<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p>
	</footer>

	*/
</script>

<div class="app">

	<box>Hello</box>

	<main>
		<slot/>
	</main>

	<box>
		<div>Hello World !</div>
		<main>Hello World !</main>
		<div>Hello World !</div>


	</box>

</div>

<style>
  div {
		border: solid 5px blue;
		border-radius: 15px;
	}

	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		border: solid 10px orange;
		border-radius: 25px;
		box-sizing: border-box; /* permet de prendre en compte l'epaisseur des border */
	}
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 0rem;
		box-sizing: border-box;
		border: solid 10px green;
		border-radius: 15px;
		width: 100%;
	}
	box {
		display: flex;
		flex-direction: column;
		height: 20vh;

		justify-content: center; /* vertical align */
		align-items: center; /* horizontal align */

		border: solid 5px red;
		border-radius: 15px;
		overflow: scroll;
	}
	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}
	footer a {
		font-weight: bold;
	}
	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
