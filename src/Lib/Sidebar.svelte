<script>
import Product from './Product.svelte';
const products = [ {}, {}, ];
</script>

<div class="sidebar">
	<h1>Recently Viewed:</h1>
	{#each products as p}
		<div class="product">
			<Product {...p} />
		</div>
	{/each}
</div>

<style>
.sidebar {
	border-left: 1px solid #c2ceb0;
	padding: 1rem;
	position: sticky;
	top: 0;
	height: 100vh;
}

h1 {
	text-transform: uppercase;
	letter-spacing: 0.25px;
	margin-bottom: 0.75rem;
	text-align: center;
}

.product + .product {
	margin-top: 0.5rem;
}
</style>
