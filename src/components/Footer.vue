<template>
	<footer>
		<Top />
		<Middle />
		<Bottom />
	</footer>
</template>

<script>
import Top from "./Top.vue";
import Middle from "./Middle.vue";
import Bottom from "./Bottom.vue";

export default {
	name: "Footer",
	components: {
		Top,
		Middle,
		Bottom,
	},
};
</script>

<style scoped lang="scss"></style>
