<script>
	let fruits = [
		{name: "Apple", color: "red", amount: 5, id: 1},
		{name: "Banana", color: "yellow", amount: 7, id: 2},
		{name: "Grape", color: "purple", amount: 3, id: 3},
	]
</script>

<main>
	<div class="card">
		<h5>{fruits[0].name}</h5>
		<p>{fruits[0].color}</p>
	</div>
</main>

<style>
	.card {
		padding: 8px;
		border-radius: 20px;
		border: 2px solid gray;
	}
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