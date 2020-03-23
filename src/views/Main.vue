<template>
	<section class="main">
		<Head></Head>
		<!-- <Colors></Colors> -->
	</section>
</template>

<script lang="ts">
import Vue from "vue";
import Head from "@/components/Main/Head.vue";
import Colors from "@/components/Main/Colors.vue";
export default Vue.extend({
	components: {
		Head,
		Colors
	}
});
</script>

<style lang="scss">
.main {
	width: 100%;
	max-width: 1200px;
	margin: 0 auto;
	padding: 40px;
}
</style>