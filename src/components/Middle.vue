<template>
	<div id="middle-header">
		<div class="container">
			<nav id="footer-nav" class="col-6">
				<div class="nav-list">
					<h5>DC COMICS</h5>
					<ul>
						<li v-for="(product, index) in products" :key="index">
							<a href="#">{{ product }}</a>
						</li>
					</ul>
					<h5>SHOP</h5>
					<ul>
						<li v-for="(shop, index) in shops" :key="index">
							<a href="#">{{ shop }}</a>
						</li>
					</ul>
				</div>
				<div class="nav-list">
					<h5>DC</h5>
					<ul>
						<li v-for="(dc, index) in dcs" :key="index">
							<a href="#">{{ dc }}</a>
						</li>
					</ul>
				</div>
				<div class="nav-list">
					<h5>SITES</h5>
					<ul>
						<li v-for="(site, index) in sites" :key="index">
							<a href="#">{{ site }}</a>
						</li>
					</ul>
				</div>
			</nav>
			<div id="col-logo" class="col-6"></div>
		</div>
	</div>
</template>

<script>
export default {
	name: "Middle",
	data() {
		return {
			products: ["Charaters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
			shops: ["Shop DC", "Shop DC Collectibles"],
			dcs: ["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Ratings", "Terms Of Use", "Privacy Policy (New)", "Contact Us"],
			sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
		};
	},
};
</script>

<style scoped lang="scss">
#middle-header {
	height: 100%;
	background-image: url(../assets/img/footer-bg.jpg);
	background-repeat: no-repeat;
	background-size: cover;
}

.container {
	display: flex;
	.col-6 {
		width: 50%;
		height: 300px;
	}
}

.nav-list {
	width: calc(80% / 3);
	height: 100%;
	padding: 30px 10px;
	h5 {
		color: white;
	}
	ul {
		list-style-type: none;
		margin-bottom: 30px;
		li a {
			color: grey;
			font-size: 10px;
			&:hover {
				text-decoration: underline;
			}
		}
	}
}

#footer-nav {
	display: flex;
}

#col-logo {
	background-image: url(../assets/img/dc-logo-bg.png);
	background-position: center;
	background-size: cover;
}
</style>
