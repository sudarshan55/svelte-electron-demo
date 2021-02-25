<script>
	export let name;

	let something;
</script>

<main>
	<h1>Hello {name}!</h1>

	<p> {something ? something : "Type Here Something "}</p>

	<input type="text" bind:value={something} placeholder ="Enter Something">

</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}
	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>