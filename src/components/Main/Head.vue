<template>
	<article class="head">
		<img src="@/assets/undraw_web_developer_p3e5.svg" class="head__img" />
		<div class="head__content">
			<h1>Andy0414</h1>
			<p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ipsam aliquam saepe enim reprehenderit ullam, amet fugiat eveniet consequatur ipsa autem qui placeat inventore facilis tenetur earum veritatis mollitia officiis repudiandae!</p>
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