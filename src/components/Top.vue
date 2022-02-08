<template>
	<div id="top-footer">
		<div class="container">
			<ul>
				<li class="card" v-for="(product, index) in products" :key="index">
					<img :src="require('../assets/img/' + product.img)" />
					<p>{{ product.text }}</p>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
export default {
	name: "Top",
	data() {
		return {
			products: [
				{ img: "buy-comics-digital-comics.png", text: "DIGITAL COMICS" },
				{ img: "buy-comics-merchandise.png", text: "DC MERCHANDISE" },
				{ img: "buy-comics-shop-locator.png", text: "SUBSCRIPTION" },
				{ img: "buy-comics-digital-comics.png", text: "COMIC SHOP LOCATOR" },
				{ img: "buy-comics-subscriptions.png", text: "DC POWER VISA" },
			],
		};
	},
};
</script>

<style scoped lang="scss">
#top-footer {
	height: 100px;
	background-color: var(--primary-color);
}

ul {
	list-style-type: none;
	display: flex;
	li {
		display: flex;
	}
}
</style>
