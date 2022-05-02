<template>
	<!-- First row of landing page (hero image with title and logo + button) -->
	<div class="row">
		<div class="hero">
			<div class="container">
				<!-- Logo in top left corner -->
				<img src="../assets/logo-white.svg" class="logo">
			</div>
			<!-- Fade in effect for title on hero -->
			<transition class="fade-enter-active">
				<div class="title text-white">
					<!-- Custom outline text -->
					<h1 class="titleTextOutline">WELCOME TO<br></h1>
					<h1 class="titleText">Rooster Grin</h1>
					<!-- Call to Action -->
					<button type="button" class="btn btn-primary">BUTTON BUTTON</button>
				</div>
			</transition>
		</div>
	</div>
</template>


<script>
export default {
  name: 'JumbotronItem',
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Londrina+Outline&display=swap');
.btn{
	background-color:#c05ee6;
	border-color: #1b181c;
	position: relative;
	border-radius: 0;
	padding-top: 1vh;
	padding-bottom: 1vh;
}
@media screen and (min-width: 768px){

.hero {
		background-image: url("../assets/hero.jpg");
		background-attachment: fixed;
		padding:0;
		background-position: top;
		background-repeat: no-repeat;
		background-size: 100% 100%;
		height:60em;
		min-width: 25em;
		min-height: 25em;
	}
	.logo{
	z-index: 2;
	position: relative;
	text-align: left;
	padding-left: 30px;
	padding-bottom: 0;
	padding-right: 0;
	width: 15em; 
	height: 15em;
}
.container {
	position: absolute;
	justify-content: left;
	align-items: left;
	max-width: 10em; 
	max-height: 10em;

}
.fade-enter-active {
  animation: go 2.5s;
}
img {
	position: absolute;
	max-height: 10em;
	max-width: 20em;
	align-items: left;
	justify-content: left;
}
.title{
	z-index: 2;
	position: relative;
	padding-top: 20em;
	padding-bottom:20em;
	justify-content: center;
	align-items: center;
	height:100%;
	width:100%;
	margin:auto;
}
.titleText{
	font-weight: bold;
	font-size: 3em;
  align-items: center;
  justify-content: center;
  text-align: center;
  line-height: 1;
  padding-bottom: 2vh;
  margin: 0;
  color: white;
}
.titleTextOutline{
	font-weight: bold;
	font-family: 'Londrina Outline', cursive;
	font-size: 3.5em;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  line-height: 1;
  padding: 0;
  margin: 0;
  padding-top: 10%;
  color: white;
}

 @keyframes go{
	from {
		opacity:0;
	}
	to{
		opacity:1;
	}
}
}
/*mobile*/
@media screen and (max-width: 767px){

.hero {
		background-image: url("../assets/hero.jpg");
		padding:0;
		background-position: center center;
		background-repeat: no-repeat;
		background-size: 100% 100%;
		height:60em;
	}

	.logo{
	z-index: 2;
	position: relative;
	text-align: center;
	padding-left: 30px;
	padding-bottom: 0;
	padding-right: 0;
	width: 15em; 
	height: 15em;
	margin:auto;
}

	.container {
	position: absolute;
	justify-content: center;
	align-items: center;
	width: 100%;
}
.fade-enter-active {
  animation: go 2.5s;
}
img {
	position: absolute;
	max-height: 10em;
	max-width: 20em;
	align-items: left;
	justify-content: left;
}
.title{
	z-index: 2;
	position: relative;
	padding-top: 20em;
	padding-bottom:20em;
	justify-content: center;
	align-items: center;
	height:100%;
	width:100%;
	margin:auto;
}
.titleText{
	font-weight: bold;
	font-size: 3em;
  align-items: center;
  justify-content: center;
  text-align: center;
  line-height: 1;
  padding-bottom: 2vh;
  margin: 0;
  color: white;
}
.titleTextOutline{
	font-weight: bold;
	font-family: 'Londrina Outline', cursive;
	font-size: 3.5em;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  line-height: 1;
  padding: 0;
  margin: 0;
  padding-top: 10%;
  color: white;
}

 @keyframes go{
	from {
		opacity:0;
	}
	to{
		opacity:1;
	}
}
}

</style>
