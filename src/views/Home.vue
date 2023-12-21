<template>
  <div id="app">
    <Sidebar />
    <Carousel />
  </div>
</template>

<script>
import Sidebar from '../components/Sidebar.vue'
import Carousel from '../components/Carousel.vue'

export default {
  name: 'App',
  components: {
    Sidebar,
    Carousel
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
