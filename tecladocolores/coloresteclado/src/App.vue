<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <!--HelloWorld msg="Welcome to Your Vue.js App"/-->
    <tecladocolor/>
  </div>
</template>

<script>
import tecladocolor from './components/tecldo.vue'

export default {
  name: 'App',
  components: {
    tecladocolor
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
