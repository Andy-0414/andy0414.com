<template>
	<article class="head">
		<img src="@/assets/undraw_web_developer_p3e5.svg" class="head__img" alt="profile_image" />
		<div class="head__content">
			<h1>Andy0414</h1>
			<p>Full Stack Web Developer</p>
			<p class="head__content__icons">
				<a
					class="head__content__iconbox"
					href="mailto:pjh8667@gmail.com"
					target="_blank"
					rel="noreferrer"
				>
					<span style="display:none">email</span>
					<i class="head__content__iconbox__icons mdi mdi-email"></i>
				</a>
				<a
					class="head__content__iconbox"
					href="https://github.com/Andy-0414"
					target="_blank"
					rel="noreferrer"
				>
					<span style="display:none">github</span>
					<i class="head__content__iconbox__icons mdi mdi-github"></i>
				</a>
				<a
					class="head__content__iconbox"
					href="https://www.facebook.com/profile.php?id=100006359646561"
					target="_blank"
					rel="noreferrer"
				>
					<span style="display:none">facebook</span>
					<i class="head__content__iconbox__icons mdi mdi-facebook"></i>
				</a>
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
	text-align: center;
	.head__img {
		max-width: 100vw;
		width: 200px;
		height: 200px;
		border-radius: 100%;
		box-shadow: 0 2px 4px -1px rgba(0, 0, 0, 0.2),
			0 4px 5px 0 rgba(0, 0, 0, 0.14), 0 1px 10px 0 rgba(0, 0, 0, 0.12);
		background-color: $background-color;
	}
	.head__content {
		padding: 20px;
		p {
			margin-top: 10px;
		}
		.head__content__icons {
			display: flex;
			justify-content: space-around;
			width: 100%;
			.head__content__iconbox {
				background: none;
				border: none;
				color: white;
				outline: none;
				width: 60px;
				height: 60px;
				border-radius: 100%;

				display: flex;
				justify-content: center;
				align-items: center;

				transition: 0.2s;
				&:hover {
					background-color: $background-color;
				}
				.head__content__iconbox__icons {
					font-size: 40px;
				}
			}
		}
	}
}
</style>