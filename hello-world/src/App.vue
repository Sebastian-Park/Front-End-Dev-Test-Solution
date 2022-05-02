<template>
 <div id="app">
  <JumbotronItem />
  <GridItem />
  <JumbotronItem2 />
  <GridItem2 />
  <JumbotronItem3 />
  <GridItem3 />
  <FooterItem />
 </div>
</template>

<script>
import JumbotronItem from './components/JumbotronItem.vue'
import JumbotronItem2 from './components/JumbotronItem2.vue'
import JumbotronItem3 from './components/JumbotronItem3.vue'
import GridItem from './components/GridItem.vue'
import GridItem2 from './components/GridItem2.vue'
import GridItem3 from './components/GridItem3.vue'
import FooterItem from './components/FooterItem.vue'

export default {
  name: 'App',
  components: {
    JumbotronItem,
    JumbotronItem2,
    JumbotronItem3,
    GridItem,
    GridItem2,
    GridItem3,
    FooterItem,
  },
};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
