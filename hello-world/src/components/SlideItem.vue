<template>
	<div class="slide">
		<transition name="slide">
			<slot/>
		</transition>
	</div>
</template>


<script>
export default {
  name: 'GridItem',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
