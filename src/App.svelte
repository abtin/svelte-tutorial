<script>
	let name="";
	let src="favicon.png"

	const resetValue = () => {
		name = "Unknown"
	}
</script>

<main>
	<h1>Hello {name}!</h1>
	<input type="text" bind:value={name}>
	<button on:click={resetValue}>Reset to unknown</button>
	<img {src} alt="Svelte icon">
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	h1 {
		font-size: 72px;
		text-align: center;
	}
	h3 {
		font-size: 30px;
	}
</style>