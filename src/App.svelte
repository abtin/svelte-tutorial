<script>
	let name="Steve";
	let src="favicon.png"
</script>

<main>
	<h1>Hello {name}!</h1>
	<img src={src} alt="Svelte icon">
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