<template>
  <div id="app">
    <div class="jumbotron-fluid header">
      <h1 class="display-4">Commute Compromiser</h1>
      <p class="lead">The tool to help you figure out where to live. </p>
    </div>
    <p class="instructions">Enter 2 addresses and Commute Compromiser will help you optimize your commutes.</p>
    <CommuteCompromise></CommuteCompromise>
  </div>
</template>

<script>
import CommuteCompromise from './components/CommuteCompromise.vue'

export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }, 
  components: {
    CommuteCompromise
  }
}
</script>

<style lang="scss">
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: rgb(12, 6, 54); 
  background-color: rgb(83, 186, 131);
}

.header {
  color: rgb(159, 217, 107);
  background-color: rgb(5, 155, 154); 
  padding-top: 20px; 
  padding-bottom: 10px; 
}

.instructions {
  padding-top: 25px; 
}
</style>
