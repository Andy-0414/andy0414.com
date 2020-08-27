<template>
	<article class="head">
		<transition name="fade">
			<img
				v-if="show"
				src="@/assets/undraw_web_developer_p3e5.svg"
				class="head__img"
				alt="profile_image"
			/>
		</transition>
		<div class="head__content">
			<transition name="fade">
				<h1 v-if="show">Andy0414</h1>
			</transition>
			<transition name="fade">
				<p v-if="show">Full Stack Web Developer</p>
			</transition>
			<transition name="fade">
				<p class="head__content__icons" v-if="show">
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
					<a class="head__content__iconbox" href="tel:010-7207-8667" target="_blank" rel="noreferrer">
						<span style="display:none">facebook</span>
						<i class="head__content__iconbox__icons mdi mdi-phone"></i>
					</a>
				</p>
			</transition>
		</div>
	</article>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
	data() {
		return {
			show: false,
		};
	},
	mounted() {
		setTimeout(() => {
			this.show = true;
		}, 200);
	},
});
</script>

<style lang="scss" scoped>
.fade-enter-active {
	transition: 1s;
}
.fade-enter {
	transform: translateY(20px);
	opacity: 0;
}
.fade-enter-to {
	transform: translateY(0);
	opacity: 1;
}
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
		h1 {
			transition-delay: 0.2s;
		}
		p {
			transition-delay: 0.4s;

			margin-top: 10px;
		}
		.head__content__icons {
			transition-delay: 0.6s;

			display: flex;
			justify-content: space-around;
			width: 100%;
			.head__content__iconbox {
				background: none;
				border: none;
				color: white;
				outline: none;
				width: 40px;
				height: 40px;
				border-radius: 100%;

				display: flex;
				justify-content: center;
				align-items: center;

				transition: 0.2s;
				&:hover {
					background-color: $background-color;
				}
				.head__content__iconbox__icons {
					font-size: 30px;
				}
			}
		}
	}
}
</style>