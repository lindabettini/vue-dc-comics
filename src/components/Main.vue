<template>
	<main>
		<div class="container">
			<h3>Content goes here</h3>
		</div>
	</main>
</template>

<script>
export default {
	name: "Main",
};
</script>

<style scoped lang="scss">
main {
	height: 80px;
	background-color: black;
	.container {
		display: flex;
		height: 100%;
		align-items: center;
	}
}

h3 {
	color: white;
}
</style>
