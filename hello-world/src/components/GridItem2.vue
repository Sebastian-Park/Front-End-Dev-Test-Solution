<template>
	<!-- Fourth row with title and content on left, icons and animation on right -->
	<div class="row">
		<!-- Custom Gradient for left side column -->
		<div class="col-md gradient-custom">
			<div class="hero">
				<!-- Title -->
				<div class="title">LOREM IPSUM <br/> DOLOR SIT AMET</div>
			</div>
			<!-- Content -->
			<p class="content">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
			<!-- Footnote CTA -->
			<p class="footnote"> > Lorem Ipsum</p>
		</div>
		<!-- Right side column containing icons and animations -->
		<div class="col-md">
			<div class="container">
				<!-- 4x4 grid of icons -->
				<div class="row row-icon">
					<div class="col">
						<div class="icon-object">
							<div class="icon-border">
								<img src="../assets/home-expertise.svg" class="icon">
							</div>
						</div>
						<!-- Icon 1 title -->
						<div class="icon-title">LOREM</div>
					</div>
					<div class="col">
							<div class="icon-object">
								<div class="icon-border">
									<img src="../assets/home-lab.svg" class="icon">
								</div>
							</div>
						<!-- Icon 2 title -->
						<div class="icon-title">LOREM IPSUM</div>
					</div>
				</div>
				<div class="row row-icon">
					<div class="col">
						<div class="icon-object">
							<div class="icon-border">
								<img src="../assets/home-hygiene.svg" class="icon">
							</div>
						</div>
						<!-- Icon 3 title -->
						<div class="icon-title">LOREM IPSUM</div>
					</div>
					<div class="col">
							<div class="icon-object">
								<div class="icon-border">
									<img src="../assets/home-retention.svg" class="icon">
								</div>
							</div>
						<!-- Icon 4 title -->
						<div class="icon-title">LOREM</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>


<script>
export default {
  name: 'GridItem2',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/*desktop*/
@media screen and (min-width:768px){
.col{
	margin:auto;
	padding-top:5%;
	padding-bottom: 5%;
	max-height: 100%;
}
.row-icon {
	position: relative;
	align-items: center;
	justify-content: center;
	position: relative;
	min-height: 50%;
	max-width: 100%;
	margin: 0;
}
.icon-object {
	align-items: center;
	justify-content: center;
	max-height:50%;
	max-width:50%;
	height:50%;
	width:50%;
	margin:auto;
	padding-bottom: 5%;
}
.icon-title {
	text-align: center;
	justify-content: center;
	font-weight: bolder;
	font-size: 1.2em;
}
.container{
	position:relative;
	min-height: 100%;
	align-items: center;
	justify-content: center;
	margin:auto;
	padding:1%;
	border:0;
}
.icon {
	max-height: 7em;
	max-width: 7em;
}
.icon-border{
	animation:leave .5s;
	max-height: 7em;
	max-width: 7em;
	border-style: solid;
	border-size: 2px;
	border-color: #e0a3f7;
    padding:1em;
    margin:auto;
    border-radius: 50%;
    top:0;
}
.icon-border:hover {
	animation: go .7s;
	max-height: 10em;
	max-width: 10em;
}
.
.hero{
	padding-top: 0vh;
}
.title {
	font-size: 2em;
	font-weight: bold;
	font-family: Arial;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
	padding-top:5vw;
}
.footnote {
	color:#8732a8;
	font-size: 1.5em;
	font-weight: bolder;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
}
.col-md {
	padding-right:0px;
	padding-left: 0px;
	min-height: 100%;
	padding:2%;
}
.gradient-custom {
  /* fallback for old browsers */
  background: #ffa200;

  /* Chrome 10-25, Safari 5.1-6 */
  background: -webkit-linear-gradient(to right, rgba(255, 162, 0, 0.5), rgba(118, 75, 162, 0.2));

  /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  background: linear-gradient(to right, rgba(255, 162, 0, 0.5), rgba(118, 75, 162, 0.2));
  min-height: 300px;
}
.content{
	font-size: 1em;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
}
@keyframes go{
	from {
		max-height: 7em;
		max-width: 7em;
	}
	to{
		max-height: 10em;
		max-width: 10em;
	}
}
@keyframes leave{
	from {
		max-height: 10em;
		max-width: 10em;
	}
	to{
		max-height: 7em;
		max-width: 7em;
	}
}
}

/*mobile*/
@media screen and (max-width: 767px){
	.col{
	margin:auto;
	padding-top:5%;
	padding-bottom: 5%;
	max-height: 100%;
}
.row-icon {
	position: relative;
	align-items: center;
	justify-content: center;
	position: relative;
	min-height: 100%;
	max-width: 100%;
	height: 12em;
	margin: 0;
}
.icon-object {
	align-items: center;
	justify-content: center;
	max-height:50%;
	max-width:50%;
	height:50%;
	width:50%;
	margin:auto;
	padding-bottom: 5%;
}
.icon-title {
	text-align: center;
	justify-content: center;
	font-weight: bolder; 
	font-size: 1.2em;
}
.container{
	position:relative;
	min-height: 100%;
	align-items: center;
	justify-content: center;
	margin:auto;
	padding:0;
	border:0;
}
.icon {
	max-height: 7em;
	max-width: 7em;
}
.icon-border{
	animation:leave .5s;
	max-height: 7em;
	max-width: 7em;
	border-style: solid;
	border-size: 2px;
	border-color: #e0a3f7;
    padding:1em;
    margin:auto;
    border-radius: 50%;
    top:0;
}
.icon-border:hover {
	animation: go .7s;
	max-height: 10em;
	max-width: 10em;
}
.
.hero{
	padding-top: 0vh;
}
.title {
	font-size: 2em;
	font-weight: bold;
	font-family: Arial;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
	padding-top:5vw;
}
.footnote {
	color:#8732a8;
	font-size: 1.5em;
	font-weight: bolder;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
}
.col-md {
	padding-right:0px;
	padding-left: 0px;
	min-height: 100%;
	padding:5%;
}
.gradient-custom {
  /* fallback for old browsers */
  background: #ffa200;

  /* Chrome 10-25, Safari 5.1-6 */
  background: -webkit-linear-gradient(to right, rgba(255, 162, 0, 0.5), rgba(118, 75, 162, 0.2));

  /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  background: linear-gradient(to right, rgba(255, 162, 0, 0.5), rgba(118, 75, 162, 0.2));
  min-height: 300px;
}
.content{
	font-size: 1em;
	justify-content: left;
	text-align:left;
	padding-left:10vw;
	padding-right: 7vw;
}
@keyframes go{
	from {
		max-height: 7em;
		max-width: 7em;
	}
	to{
		max-height: 10em;
		max-width: 10em;
	}
}
@keyframes leave{
	from {
		max-height: 10em;
		max-width: 10em;
	}
	to{
		max-height: 7em;
		max-width: 7em;
	}
}
}
</style>
