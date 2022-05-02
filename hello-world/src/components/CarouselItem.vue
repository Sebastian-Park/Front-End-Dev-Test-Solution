<template>
	<!-- Carousel item -->
	<div class="carousel">
		<slot :currentSlide="currentSlide"/>
		<!-- Navigation -->
		<div class="navigate">
			<!-- Left Arrow -->
			<div class="toggle-page left">
				<i @click="prevSlide" class="fa fa-angle-left"></i>
			</div>
			<!-- Right Arrow -->
			<div class="toggle-page right">
				<i @click="nextSlide" class="fa fa-angle-right"></i>
			</div>
		</div>
		<!-- Pagination -->
		<div class="pagination">
			<span v-for="(slide, index) in getSlideCount" 
			:key="index" 
			:class="{active : index + 1 === currentSlide}">
			</span>
		</div>
	</div>
</template>


<script>
import { ref, onMounted } from 'vue';
export default {
	setup(){
		const currentSlide = ref(1);
		const getSlideCount = ref(null);

		// Next Slide
		const nextSlide = () => {
			if (currentSlide.value === getSlideCount.value){
				currentSlide.value = 1;
				return
			}
			currentSlide.value += 1;
		};

		// Previous Slide
		const prevSlide = () => {
			if (currentSlide.value === 1){
				currentSlide.value = 1;
				return
			}
			currentSlide.value -= 1;
		};

		onMounted(() => {
			getSlideCount.value = document.querySelectorAll(".slide").length;
		});
		return {currentSlide, nextSlide, prevSlide, getSlideCount};
	},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.carousel {
	/*position:bottom;*/
	position: relative;
	min-height:27em;
}
span {
	cursor: pointer;
	width: 1vw;
	height: 1vw;
	border-radius: 50%;
	background-color: #808080;
	box-shadow: 0 1px 3px 0 rgba(0,0,0, 0.1), 0 1px 2px 0 rgba(0, 0, 0, 0,6);
}
.active {
	background-color: #6347c7
}
.pagination {
	position: relative;
	bottom: 1vw;
	width: 100%;
	display: flex;
	gap: 16px;
	justify-content: center;
	align-items: center;
}
.navigate {
	padding: 0 16px;
	height: 100%;
	width: 100%;
	position: relative;
	display: flex;
	justify-content: center;
	align-items: center;
	top: 50%;
}

.toggle-page {
	display: flex;
	flex: 1;
}
.right{
	justify-content: flex-end;
}

i {
	cursor: pointer;
	display: flex;
	align-items: center;
	justify-content: center;
	border-radius: 50%;
	width: 40px;
	height: 40px;
	background-color: #6347c7;
	color: #fff;
}
</style>
