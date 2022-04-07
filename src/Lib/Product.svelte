<div class="product">
	<div class="product-container">
		<figure><img src="https://www.ikea.com/us/en/images/products/fejka-artificial-potted-plant-indoor-outdoor-cactus__0935865_PE792997_S5.JPG?f=xs" />
		</figure>
		<div>
			<h3>Cactus</h3>
			<span class="price">$16.99</span>
			<p>This plant is a very good one. There is a product description that talks about plant care and other details here.</p>
			<button>Add to Cart</button>
		</div>
	</div>
</div>

<style>
img {
	width: 100%;
}

figcaption,
h3 {
	font-size: 14px;
	font-weight: 800;
	text-transform: uppercase;
	letter-spacing: 0.25px;
	margin: 0.5rem 1rem 0;
}

.price {
	display: block;
	font-size: 14px;
	margin: 0 1rem;
}

.product p {
	margin-top: 1rem;
	font-size: 13px;
	color: #555;
	margin: 0.5rem 1rem 0;

}

button {
	border: none;
	display: block;
	background: white;
	font-size: 14px;
	font-weight: 800;
	text-transform: uppercase;
	letter-spacing: 0.25px;
	padding: 0.25rem 0.5rem;
	margin: 1rem auto;
	cursor: pointer;
	background: #c2ceb0;
}

/* これはProduct を利用する側(Sidebar)に持たせるべきCSS
.sidebar .product + .product {
	margin-top: 0.5rem;
}
*/

/* CQ (=Container Query) コンテナークエリーに関連するもの */
.product {
	container: inline-size;
}

.hero .product {
	position: absolute;
	bottom: 1rem;
	right: 1rem;
	/* Slot the product card into a size */
	width: 350px;
	background: white;
}

/* Smaller version (ie. sidebar in this demo) */
/*
@container (max-width: 200px) {
	.product-container {
		border: 1px solid #c2ceb0;
		padding: 0.5rem;
		border-radius: 10px;
		display: flex;
		align-items: center;
	}

	.product-container h3 {
		letter-spacing: 0;
		width: 90px;
		overflow: hidden;
		text-overflow: ellipsis;
		white-space: pre;
		margin: 0;
	}

	.product-container span {
		margin: 0;
	}

	.product-container p,
	.product-container button {
		display: none;
	}
}
*/

/* wider sizes (i.e in hero) */
/*
@container (min-width: 350px) {
	.product-container {
		padding: 0.5rem 0 0;
		display: flex;
	}
	.product button {
		margin-left: 1rem;
	}
}
*/
</style>
