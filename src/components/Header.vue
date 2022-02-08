<template>
	<header>
		<div class="container">
			<nav>
				<div>ciao</div>
				<div>ciao</div>
			</nav>
		</div>
	</header>
</template>

<script>
export default {
	name: "Header",
};
</script>

<style scoped lang="scss">
header {
	height: 80px;
	background-color: pink;
}

nav {
	height: 100%;
	display: flex;
	justify-content: space-between;
	align-items: center;
}
</style>
