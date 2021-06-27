<script>
	import Announcement from "./Announcement.svelte";

	let fruits = [
		{name: "Apple", color: "red", amount: 5, id: 1},
		{name: "Banana", color: "yellow", amount: 7, id: 2},
		{name: "Grape", color: "purple", amount: 3, id: 3},
	]
	const deleteFruit = (id) => {
		console.log("Deleting fruit with id:", id);
		fruits = fruits.filter((f) => f.id !== id);
	}
</script>

<main>
	<Announcement />
	{#each fruits as fruit (fruit.id)}
		{#if fruit.amount > 4}
			<div class="card">
				<h5>{fruit.name}</h5>
				<p>{fruit.color}</p>
				<button on:click={() => deleteFruit(fruit.id)}>Delete</button>
			</div>
			{:else}
			<p>The amount for {fruit.name} is less than 4</p>
		{/if}
	{:else}
		<p>There are no fruit in our fruits array</p>
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