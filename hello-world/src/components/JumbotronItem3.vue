<template>
	<!-- Fifth row containing hero with title, content, and button on right half of vp -->
	<div class="row">
		<!-- Hero with background img -->
		<div class="hero">
			<div class="container">
				<div class="row row-obj">
					<div class="col-obj">
					</div>
					<div class="col">
						<!-- Title -->
						<div class="title">LOREM IPSUSM </div>
						<!-- Content -->
						<p class="content">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
						<!-- Button -->
						<div class="content">
							<button type="button" class="btn btn-primary">BUTTON BUTTON</button>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>


<script>
export default {
  name: 'JumbotronItem3',
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Londrina+Outline&display=swap');
/*desktop*/
@media screen and (min-width: 768px){
	.col-obj {
		width: 50%;
	}
	.row-obj {
		padding-top: 10%;
		padding-bottom: 10%;
	}
	.container{
		position: relative;
		height: 100%;
		margin:auto;
		padding:8em;
		padding-right:1%;
	}
	.btn{
		background-color:#ff6f00;
		border-color: #ff6f00;
		position: relative;
		border-radius: 0;
		padding-top: 1vh;
		padding-bottom: 1vh;

	}
	.hero{
		background-image: url("../assets/banner-2.jpg");
		background-attachment: fixed;
		background-position: center center;
		background-repeat: no-repeat;
		background-size: 130% 100%;
		width: 100%;
		min-height: 20em;
		height: 40em;
		padding:0;
	}
	.title{
		color:#8732a8;
		font-size: 1.8em;
		z-index: 2;
		position: relative;
		padding-bottom:5%;
		font-weight: bolder;
		justify-content: left;
		text-align:left;
		padding-left: 2vw;
	}
	.content{
		position: relative;
		font-size: 1em;
		justify-content: left;
		text-align:left;
		padding-left:2.3vw;
	}
}
/*mobile*/
@media screen and (max-width: 767px){
	.row-obj {
	padding-top: 20em;
	padding-bottom: 20em;
	height:100%;
	}
	.container{
		position: relative;
		max-height: 100%;
		margin:auto;
		height: 100%;
		background: linear-gradient(to bottom, rgba(118, 75, 162, 0.2), rgba(255, 162, 0, 0.5));
	}
	.btn{
		background-color:#ff6f00;
		border-color: #ff6f00;
		position: relative;
		border-radius: 0;
		padding-top: 1vh;
		padding-bottom: 1vh;

	}
	.hero{
		background-image: url("../assets/banner-2.jpg");
		/*background-attachment: fixed;*/
		background-position: 40% center;
		background-repeat: no-repeat;
		background-size: 400% 100%;
		width: 100%;
		min-height: 20em;
		height: 50em;
		padding:0;
	}
	.title{
		color:#8732a8;
		font-size: 1.8em;
		z-index: 2;
		position: relative;
		padding-bottom:5%;
		font-weight: bolder;
		justify-content: center;
		text-align:center;
		padding-left: 2vw;
	}
	.content{
		position: relative;
		font-size: 1em;
		justify-content: center;
		text-align:center;
		padding-left:2.3vw;
		color:#fff;
		font-weight: bold;
	}
}

</style>
