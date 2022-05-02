<template>
	<!-- Sixth row containing title and star rating on left and carousel on right -->
	<div class="row">
		<!-- Custom gradient for left side-->
		<div class="col-sm gradient-custom">
			<div class="hero">
				<!-- Title -->
				<div class="title">LOREM IPSUM <br/>DOLOR SIT AMET</div>
				<!-- Container containing star icons -->
				<div class="container">
					<i class="fa fa-star"></i>
					<i class="fa fa-star"></i>
					<i class="fa fa-star"></i>
					<i class="fa fa-star"></i>
					<i class="fa fa-star"></i>
				</div>
			</div>
		</div>
		<!-- Carousel item for right side -->
		<div class="col-sm carousel-container">
			<CarouselItem class="carousel" v-slot="{currentSlide}">
				<SlideItem v-for="(slide, index) in carouselSlides" :key="index">
					<div  v-show="currentSlide === index + 1" class="slideInfo">
						<p class="slide-title">{{slide}}</p>
						<p>{{carouselContent[index]}}</p>
					</div>
				</SlideItem>
			</CarouselItem>
		</div>
	</div>
</template>


<script>
import SlideItem from '../components/SlideItem.vue'
import CarouselItem from '../components/CarouselItem.vue'
export default {
  name: 'GridItem3',
  components: {SlideItem, CarouselItem},
  setup(){
	const carouselSlides =["John Doe", "Jane Poe", "Connie Coe"];
	const carouselContent = 
	[
		"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
		"Consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. consectetur adipiscing elit.",
		"Ut enim ad minim veniam, lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
	]

	return {carouselSlides, carouselContent};
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@media screen and (min-width: 768px){
.carousel-container {
	padding-top:0;
	padding-bottom:10vw;
	size:cover;
	min-height: 300px;
}
.fa-star {
	font-size:2em;
}
.slide-title{
	padding-top: 20%;
	color:#8732a8;
	font-size: 2em;
	font-weight: bolder;
}
.carousel {
	/*align-self:center;*/
	height: 100%;
	width: 100%;
}
.slideInfo {
	padding-bottom: 20vw;
		font-size: 1em;
		position: absolute;
		top: 0;
		left: 0;
		padding-left: 15%;
		padding-right: 15%;
		width: 100%;
		max-height: 100%;
		height:100%;
		p {
			min-width: 100%;
			height: 100%;
			object-fit: cover;
		}
	}
.fa-star{
	color: #ff6f00;
	padding-top:5px;
	padding-left: .5vw;
	padding-right:.5vw;
}
.container{
	padding-top: 1vh;
	padding-bottom: 10vh;
	padding-left:9.5vw;
	padding-right: 13vw;
	text-align: left;
}
.hero{
	height:100%;
	padding-top:25%;
	margin:auto;
}
.title {
	font-size: 3em;
	font-weight: bold;
	font-family: Arial;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
}
.col-sm {
	padding-right:0px;
	padding-left: 0px;
}
.gradient-custom {
  /* fallback for old browsers */
  background: #ffa200;

  /* Chrome 10-25, Safari 5.1-6 */
  background: -webkit-linear-gradient(to right, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));

  /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  background: linear-gradient(to right, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));
}
.content{
	font-size: 1em;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
}
}

/*mobile*/
@media screen and (max-width: 767px){
	.carousel-container {
	padding-top:0;
	padding-bottom:10vw;
	size:cover;
	min-height: 300px;
}
.slide-title{
	padding-top: 5vh;
	color:#8732a8;
	font-size: 2em;
	font-weight: bolder;
}
.carousel {
	/*align-self:center;*/
	height: 100%;
	width: 100%;
}
.slideInfo {
	padding-bottom: 20vw;
		font-size: 1em;
		position: absolute;
		top: 0;
		left: 0;
		padding-left: 15%;
		padding-right: 15%;
		width: 100%;
		max-height: 100%;
		height:100%;
		p {
			min-width: 100%;
			height: 100%;
			object-fit: cover;
		}
	}
.fa-star{
	color: #ff6f00;
	padding-top:5px;
	padding-left: .5vw;
	padding-right:.5vw;
}
.container{
	padding-top: 1vh;
	padding-bottom: 10vh;
	padding-left:9.5vw;
	padding-right: 13vw;
	text-align: left;
}
.hero{
	padding-top: 30%;
}
.title {
	font-size: 2em;
	font-weight: bold;
	font-family: Arial;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
}
.col-sm {
	padding-right:0px;
	padding-left: 0px;
}
.gradient-custom {
  /* fallback for old browsers */
  background: #ffa200;

  /* Chrome 10-25, Safari 5.1-6 */
  background: -webkit-linear-gradient(to right, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));

  /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  background: linear-gradient(to right, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));
}
.content{
	font-size: 1em;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
}
}

</style>
