<template>
	<Layout>
		<!-- Learn how to use images here: https://gridsome.org/docs/images -->
		<!-- <g-image alt="Example image" src="~/images/bg2.jpg" width="100%" /> -->
		<!-- :src="require(`!!assets-loader!@images/IMG_2${1 + 1}.jpg`)"  -->

		<div class="bghero">
			<div class="container mx-auto px-4">
				<h1 class="text-5xl py-80">Monika!</h1>
			</div>
		</div>

		<!-- <carousel-3d
			:controls-visible="true"
			:controls-prev-html="'&#10092;'"
			:controls-next-html="'&#10093;'"
			:controls-width="30"
			:controls-height="60"
			:autoplay="true"
			:autoplay-timeout="5000"
			:display="3"
			:width="600"
			:height="400"
		>
			<slide v-for="(slide, i) in slides" :index="i" :key="i">
				<g-image
					alt="Example image"
					:src="'IMG_' + parseInt(i + 1) + '.jpg'"
					width="100%"
				/>
			</slide>
		</carousel-3d> -->

		<p>
			Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur
			excepturi labore tempore expedita, et iste tenetur suscipit
			explicabo! Dolores, aperiam non officia eos quod asperiores
		</p>

		<p class="home-links">
			<a href="https://gridsome.org/docs/" target="_blank" rel="noopener"
				>Gridsome Docs</a
			>
			<a
				href="https://github.com/gridsome/gridsome"
				target="_blank"
				rel="noopener"
				>GitHub</a
			>
		</p>
	</Layout>
</template>

<script>
// import { Carousel3d, Slide } from "vue-carousel-3d";

export default {
	data() {
		return {
			slides: 20,
		};
	},
	// components: {
	// 	Carousel: () =>
	// 		import("vue-carousel-3d")
	// 			.then((m) => m.Carousel3d)
	// 			.catch(),
	// 	Slide: () =>
	// 		import("vue-carousel-3d")
	// 			.then((m) => m.Slide)
	// 			.catch(),
	// },
	computed: {
		setImage: function() {
			return this.image ? "/bg.jpg" : "/bg.jpg" + this.image + "sadf";
		},
	},
	metaInfo: {
		title: "Hello, world!",
	},
};
</script>

<style>
.home-links a {
	margin-right: 1rem;
}
.bghero {
	background-image: url(../images/bg2.jpg);
	background-repeat: no-repeat;
	background-size: cover;
	color: white;
}
h1 {
	min-height: 400px;
}
</style>
