<template>
  <div id="app">
    <Groceries/>
  </div>
</template>

<script>
import Groceries from './components/Groceries.vue'

export default {
  name: 'app',
  components: {
    Groceries
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
