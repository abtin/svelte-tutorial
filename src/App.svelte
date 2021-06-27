<script>
	let firstName="";
	let lastName="";
	let src="favicon.png"

	$: fullName = `${firstName} ${lastName}`
</script>

<main>
	<h1>Hello {fullName}!</h1>

	<label for="fistName">First Name</label>
	<input type="text" bind:value={firstName}>

	<label for="lastName">Last Name</label>
	<input type="text" bind:value={lastName}>
	
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