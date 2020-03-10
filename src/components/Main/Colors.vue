<template>
<!-- Dev Colors (TEST) -->
	<article class="colors">
		<h1 class="color-title">
			Colors
			<a href="https://undraw.co/illustrations" target="_blank">(REF)</a>
		</h1>
		<div class="color-item">
			<div class="color-item__color color1"></div>
			<div class="color-item__content">#536dfe</div>
		</div>
		<div class="color-item">
			<div class="color-item__color color2"></div>
			<div class="color-item__content">#f50057</div>
		</div>
		<div class="color-item">
			<div class="color-item__color color3"></div>
			<div class="color-item__content">#f9a826</div>
		</div>
	</article>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({});
</script>

<style lang="scss" scoped>
.color-title {
	font-size: 40px;
}
.color-item {
	display: flex;
	justify-content: space-between;
	align-items: center;
	width: 200px;
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