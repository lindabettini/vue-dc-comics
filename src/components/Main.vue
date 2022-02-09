<template>
	<main>
		<div class="container">
			<section id="current-series">
				<div class="section-title"><h3>CURRENT SERIES</h3></div>
				<ul id="serie-cards">
					<li class="serie-card" v-for="(serie, index) in series" :key="index">
						<figure>
							<img :src="serie.thumb" alt="serie.series" />
						</figure>
						<a href="#">{{ serie.series }}</a>
					</li>
				</ul>
				<div class="btn-container"><button class="primary-btn">LOAD MORE</button></div>
			</section>
		</div>
	</main>
</template>

<script>
export default {
	name: "Main",
	props: ["series"],
};
</script>

<style scoped lang="scss">
main {
	background-color: rgb(12, 12, 12);
	.container {
		display: flex;
		align-items: center;
	}
}

#current-series {
	padding-bottom: 20px;
}

#serie-cards {
	display: flex;
	flex-wrap: wrap;
}

.section-title {
	color: white;
	width: 200px;
	text-align: center;
	h3 {
		background-color: var(--primary-color);
		padding: 10px;
		position: relative;
		bottom: 20px;
	}
}

ul {
	list-style: none;
	display: flex;
	li {
		color: white;
		padding: 10px;
		width: calc(100% / 6);
		figure {
			height: 150px;
			width: 150px;
			overflow: hidden;
			margin-bottom: 15px;
		}
		a {
			color: white;
			text-decoration: none;
		}
	}
}

.btn-container {
	display: flex;
	justify-content: center;
	button {
		padding: 7px 40px;
		margin-top: 30px;
		cursor: pointer;
	}
}
</style>
