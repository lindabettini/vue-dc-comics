<template>
	<footer>
		<FooterTop />
		<FooterMiddle />
		<FooterBottom />
	</footer>
</template>

<script>
import FooterTop from "./FooterTop.vue";
import FooterMiddle from "./FooterMiddle.vue";
import FooterBottom from "./FooterBottom.vue";

export default {
	name: "Footer",
	components: {
		FooterTop,
		FooterMiddle,
		FooterBottom,
	},
};
</script>

<style scoped lang="scss"></style>
