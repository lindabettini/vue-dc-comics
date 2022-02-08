<template>
	<header>
		<div class="container">
			<nav>
				<figure>
					<img src="../assets/img/dc-logo.png" alt="DC logo" />
				</figure>
				<ul>
					<li v-for="(link, index) in links" :key="index">
						<a :href="link.url">{{ link.text }}</a>
					</li>
				</ul>
			</nav>
		</div>
	</header>
</template>

<script>
export default {
	name: "Header",
	data() {
		return {
			links: [
				{ text: "Characters", url: "#", active: false },
				{ text: "Comics", url: "#", active: false },
				{ text: "Movies", url: "#", active: false },
				{ text: "Tv", url: "#", active: false },
				{ text: "Games", url: "#", active: false },
				{ text: "Collectibles", url: "#", active: false },
				{ text: "Video", url: "#", active: false },
				{ text: "Fans", url: "#", active: false },
				{ text: "News", url: "#", active: false },
				{ text: "Shop", url: "#", active: false },
			],
		};
	},
};
</script>

<style scoped lang="scss">
header {
	height: 80px;
	background-color: white;
	.container {
		height: 100%;
		nav {
			height: 100%;
			display: flex;
			justify-content: space-between;
			align-items: center;
		}
	}
}

img {
	width: 60px;
}

ul {
	list-style-type: none;
	li {
		display: inline-block;
	}
	li a {
		padding: 10px;
		&:hover {
			border-bottom: 3px solid var(--primary-color);
		}
	}
}
</style>
