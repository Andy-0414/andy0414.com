<template>
	<div class="main">
		<h1 class="color-title">
			Colors
			<a href="https://undraw.co/illustrations">(REF)</a>
		</h1>
		<section class="color-item">
			<div class="color-item__color color1"></div>
			<div class="color-item__content">#536dfe</div>
		</section>
		<section class="color-item">
			<div class="color-item__color color2"></div>
			<div class="color-item__content">#f50057</div>
		</section>
		<section class="color-item">
			<div class="color-item__color color3"></div>
			<div class="color-item__content">#f9a826</div>
		</section>
	</div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.main {
	width: 300px;
	margin: 0 auto;
	padding: 40px;
}
.color-title {
	font-size: 40px;
	text-align: center;
}
.color-item {
	display: flex;
	justify-content: space-between;
	align-items: center;
	width: 100%;
	padding: 20px;

	background-color: $deep-background-color;
	box-shadow: 0 2px 10px rgba(32, 32, 32, 0.5);
	margin: 20px 0;
}
.color-item__color {
	width: 80px;
	height: 80px;

	&.color1 {
		background-color: $main-color;
	}
	&.color2 {
		background-color: $point-color;
	}
	&.color3 {
		background-color: $highlight-color;
	}
}
</style>