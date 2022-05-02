<template>
	<!-- Third row - hero image with title and button -->
	<div class="row">
		<div class="hero">
			<div class="container">
				<div class="row-obj">
					<div class="col">
						<div class="title">
							<h1 class="title">LOREM IPSUSM <br/>
								<button type="button" class="btn btn-primary">BUTTON BUTTON</button>
							</h1>
						</div>
					</div>
					<!-- <div class="col"></div> -->
				</div>
			</div>
		</div>
	</div>
</template>


<script>
export default {
  name: 'JumbotronItem2',
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Londrina+Outline&display=swap');
/*desktop*/
@media screen and (min-width: 768px){

	.row-obj {
		position: relative;
		max-width: 100;
		height: 100%;
		align-items: center;
		justify-content: center;
	}
	.container{
		padding:0;
		margin:0;
		min-width: 100%;
		height: 100%;
		margin: auto;
	}
	.col {
		max-width: 50%;
		height: 100%;
		position: relative;
		padding:0;
		border:0;
		align-items: center;
		justify-content: center;
		padding-top:10em;
		padding-bottom: 10em;
		padding-left:.5vw;
		
	}
	.btn{
		background-color:#ff6f00;
		border-color: #ff6f00;
		position: relative;
		border-radius: 0;
		padding-top: 1vh;
		padding-bottom: 1vh;
		font-size: .5em;
		margin:20px;
	}
	.hero{
		position: relative;
		background-image: url("../assets/banner-1.jpg");
		background-position: top;
		background-attachment: fixed;
		background-repeat: no-repeat;
		background-size: 100% 100%;
		width: 100%;
		/*height: 100%;*/
		min-height: 10em;
		/*height: 40em;*/
		padding:0;
	}
	.title{
		color:#8732a8;
		font-size: 1.5em;
		z-index: 2;
		font-weight: bolder;
		position: relative;
		align-items: center;
		justify-content: center;
		padding:2em;
	}
}
@media screen and (max-width: 767px) {
	.row-obj {
		position: relative;
		max-width: 100;
		height: 100%;
		align-items: center;
		justify-content: center;
	}
	.container{
		padding:0;
		margin:0;
		min-width: 100%;
		height: 100%;
		margin: auto;
	}
	.col {
		max-width: 100%;
		height: 100%;
		position: relative;
		padding:0;
		border:0;
		align-items: center;
		justify-content: center;
		padding-top:20em;
		padding-bottom: 20em;
		padding-left:.5vw;
		
	}
	.btn{
		background-color:#ff6f00;
		border-color: #ff6f00;
		position: relative;
		border-radius: 0;
		padding-top: 1vh;
		padding-bottom: 1vh;
		font-size: .5em;
		margin: 1em;
	}
	.hero{
		/*background-attachment: fixed;*/
		background-image: url("../assets/banner-1.jpg");
		background-position:60% center;
		background-repeat: no-repeat;
		background-size: 350% 100%;
		width: 100%;
		min-height: 10em;
		height: 60em;
		padding:0;
	}
	.title{
		color:#8732a8;
		font-size: 1.5em;
		z-index: 2;
		font-weight: bolder;
		position: relative;
		align-items: center;
		justify-content: center;
		padding:2em;
		padding-right:0;
		padding-left: 0;
	}
}

</style>
