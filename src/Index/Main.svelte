<script>
import Product from '../Lib/Product.svelte';
const products = [ {}, {}, {}, {}, {}, {}, {}, ];
</script>

<div class="main">
	{#each products as p}
		<Product {...p} />
	{/each}
</div>

<style>
.main {
	padding: 2rem 3rem;
	display: grid;
	grid-gap: 4rem 2rem;
	grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
}
</style>
