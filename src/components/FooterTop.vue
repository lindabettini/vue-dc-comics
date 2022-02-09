<template>
	<div id="top-footer">
		<div class="container">
			<ul>
				<li class="card" v-for="(product, index) in products" :key="index">
					<img :src="require('../assets/img/' + product.img)" />
					<a :href="product.link">{{ product.text }}</a>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
export default {
	name: "FooterTop",
	data() {
		return {
			products: [
				{ img: "buy-comics-digital-comics.png", text: "DIGITAL COMICS", link: "#" },
				{ img: "buy-comics-merchandise.png", text: "DC MERCHANDISE", link: "#" },
				{ img: "buy-comics-subscriptions.png", text: "SUBSCRIPTION", link: "#" },
				{ img: "buy-comics-shop-locator.png", text: "COMIC SHOP LOCATOR", link: "#" },
				{ img: "buy-dc-power-visa.svg", text: "DC POWER VISA", link: "#" },
			],
		};
	},
};
</script>

<style scoped lang="scss">
@import "@/sass/_vars.scss";
#top-footer {
	height: 100px;
	background-color: $main-color;
	display: flex;
	justify-content: center;
	align-items: center;
}

ul {
	height: 100%;
	list-style-type: none;
	display: flex;
	justify-content: center;
	align-items: center;
	li {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 20px;
		img {
			width: auto;
			height: 40px;
			margin: 5px;
		}
		a {
			color: white;
			font-size: 10px;
		}
	}
}
</style>
