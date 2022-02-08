<template>
	<div id="bottom-footer">
		<div class="container">
			<div id="sing-up" class="col-6">
				<button class="clickable">SING-UP NOW!</button>
			</div>
			<div id="socials" class="col-6">
				<h4>FOLLOW US</h4>
				<a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook" /></a>
				<a href="#"><img src="../assets/img/footer-twitter.png" alt="Facebook" /></a>
				<a href="#"><img src="../assets/img/footer-youtube.png" alt="Facebook" /></a>
				<a href="#"><img src="../assets/img/footer-pinterest.png" alt="Facebook" /></a>
				<a href="#"><img src="../assets/img/footer-periscope.png" alt="Facebook" /></a>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "Bottom",
};
</script>

<style scoped lang="scss">
#bottom-footer {
	height: 80px;
	background-color: rgb(34, 34, 34);
	.container {
		display: flex;
		justify-content: space-between;
		align-items: center;
		height: 100%;
	}
}

.col-6 {
	width: 50%;
	height: 100%;
	display: flex;
	align-items: center;
}

#socials {
	justify-content: flex-end;
}

a {
	padding: 5px;
}

button {
	background-color: transparent;
	padding: 7px;
	border: 2px solid var(--primary-color);
	color: white;
}

h4 {
	color: var(--primary-color);
}
</style>
