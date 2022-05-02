<template>
	<!-- Second row item, 2-columns grid-->
	<div class="row">
		<!-- Custom gradient -->
		<div class="col-md gradient-custom">
			<!-- Title -->
			<div class="title">LOREM IPSUM</div>
			<!-- Content -->
			<p class="content">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
			<!-- Footnote CTA -->
			<p class="footnote"> > Lorem Ipsum</p>
		</div>
		<!-- Right side column with image -->
		<div class="col-md">
			<img src="../assets/img-1.jpg" style="width:100%;">
		</div>
	</div>
</template>


<script>
export default {
  name: 'GridItem',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/*desktop*/
@media screen and (min-width:768px){

	img {
		min-height: 100%;
		min-width: 100%;
	}
	.title {
		font-weight:bold;
		color:#8732a8;
		font-size: 2em;
		font-weight: bolder;
		justify-content: left;
		text-align:left;
		padding-left:10vw;
		padding-right: 7vw;
		padding-top:10%;
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
		padding-right:0;
		padding-left: 0px;
		min-width: 25em;
		min-height: 20em;
	}
	.gradient-custom {
	/* fallback for old browsers */
	background: #ffa200;

	/* Chrome 10-25, Safari 5.1-6 */
	background: -webkit-linear-gradient(to right, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));

	/* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
	background: linear-gradient(to right, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));
	padding:5%;
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

	img {
		min-height: 100%;
		min-width: 100%;
	}
	.title {
		font-weight:bold;
		color:#8732a8;
		font-size: 2em;
		font-weight: bolder;
		justify-content: left;
		text-align:left;
		padding-left:10vw;
		padding-right: 7vw;
		padding-top:10%;
	}
	.footnote {
		color:#8732a8;
		font-size: 1.5em;
		font-weight: bolder;
		justify-content: left;
		text-align:left;
		padding-left:10vw;
		padding-right: 7vw;
		padding-bottom: 5%;
	}
	.col-md {
		padding-right:0;
		padding-left: 0px;
		min-width: 25em;
		min-height: 20em;
	}
	.gradient-custom {
	/* fallback for old browsers */
	background: #ffa200;

	/* Chrome 10-25, Safari 5.1-6 */
	background: -webkit-linear-gradient(to right, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));

	/* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
	background: linear-gradient(to right, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));
	padding:2em;
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
