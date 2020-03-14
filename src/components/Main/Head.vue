<template>
	<article class="head">
		<img src="@/assets/undraw_web_developer_p3e5.svg" class="head__img" />
		<div class="head__content">
			<h1>Andy0414</h1>
			<p>Full Stack Web Developer</p>
			<p>
				GITHUB:
				<a href="https://github.com/andy-0414">https://github.com/andy-0414</a>
			</p>
		</div>
	</article>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({});
</script>

<style lang="scss" scoped>
.head {
	width: 100%;
	display: flex;
	.head__img {
		width: 40%;
	}
	.head__content {
		padding: 20px;
	}
}
</style>