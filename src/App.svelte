<script>
	let fruits = [
		{name: "Apple", color: "red", amount: 5, id: 1},
		{name: "Banana", color: "yellow", amount: 7, id: 2},
		{name: "Grape", color: "purple", amount: 3, id: 3},
	]
</script>

<main>
	{#each fruits as fruit}
		<div class="card">
			<h5>{fruit.name}</h5>
			<p>{fruit.color}</p>
		</div>
	{/each}
</main>

<style>
	h5, p {
		margin: 4px 0px;
	}
	.card {
		min-width: 400px;
		padding: 8px;
		border-radius: 20px;
		border: 2px solid gray;
		margin-top: 8px;
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