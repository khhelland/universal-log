<script>
	import Item from "./Item.svelte";
	let categories = ["restauranter", "bøker", "museer"];

	function add() {
		//should bring up modal for info
		categories = categories.concat("new");
	}
</script>

<main>
	<ul>
		{#each categories as category}
			<li>
				<Item>
					<span slot="name">
						{category}
					</span>
				</Item>
			</li>
		{/each}
	</ul>

	<button class="addButton" on:click={add}> Add! </button>
</main>

<style>
	.addButton {
		color: aquamarine;
	}
</style>
