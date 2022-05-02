<template>
	<!-- Footer Object to promote social media -->
	<div class="row">
		<div class="footer">
			<h2>Follow Us:</h2>
			<div class="col">
				<!-- Social media logo icons -->
				<img src="../assets/instagram.svg" class="logo">
				<img src="../assets/facebook.svg" class="logo">
			</div>
		</div>
	</div>
</template>


<script>
export default {
  name: 'FooterItem',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
	background-color: rgba(235, 235, 235, 0.3);
}
h2 {
	padding-top: 2vh;
	font-weight: bold; 
	font-color: #808080;
}
.logo {
	animation: leave ease 1s;
	padding: 15px;
	width: 7em;
	filter: invert(18%) sepia(94%) saturate(2196%) hue-rotate(271deg) brightness(93%) contrast(85%);
}
.logo:hover {
	animation:go ease 1s;
	width:8.5em;
	height:8.5em;
}

.logo svg {
	fill: currentColor;
}
@keyframes go{
	from {
		height: 7em;
		width: 7em;
	}
	to{
		height: 8.5em;
		width: 8.5em;
	}
}
@keyframes leave{
	from {
		height: 8.5em;
		width: 8.5em;
	}
	to{
		height: 7em;
		width: 7em;
	}
}
</style>
