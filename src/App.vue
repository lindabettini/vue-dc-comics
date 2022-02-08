<template>
	<div id="app">
		<Header />
	</div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
	name: "App",
	components: {
		Header,
	},
};
</script>

<style lang="scss">
* {
	padding: 0;
	margin: 0;
	box-sizing: border-box;
}

body {
	font-family: Avenir, Helvetica, Arial, sans-serif;
}

img {
	max-width: 100%;
	height: auto;
}

a {
	color: black;
	text-decoration: none;
}

// ~ Utils
.container {
	max-width: 1000px;
	margin: 0 auto;
}

.clickable {
	cursor: pointer;
}

.h-100 {
	height: 100%;
}

:root {
	--primary-color: rgb(12, 124, 236);
}
</style>
