<script>
	let name="";
	let src="favicon.png"
	let count = 0;

	const incrementCounter = () => {
		count++;
	}
	// const handleInput = (event) => {
	// 	name = event.target.value;
	// }
	const resetValue = () => {
		name = "Unknown"
	}
</script>

<main>
	<h1>Hello {name}!</h1>
<!--	<h3>Counter: {count}</h3>-->
<!--	<button on:click={incrementCounter}>Add 1 to counter</button>-->
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