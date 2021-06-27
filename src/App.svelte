<script>
	let name="Steve";
	let src="favicon.png"
	let count = 0;
</script>

<main>
	<h1>Hello {name}!</h1>
	<h3>Counter: {count}</h3>
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
</style>