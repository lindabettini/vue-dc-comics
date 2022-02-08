<template>
	<section id="content">
		<div class="container">
			<h3>Content goes here</h3>
		</div>
	</section>
</template>

<script>
export default {
	name: "Content",
};
</script>

<style scoped lang="scss">
#content {
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
