<template>
  <div>
    <circle-diagram/>
  </div>
</template>

<script>
import circleDiagram from './components/circleDiagram.vue'
export default {
  name: 'App',
  components:{
    circleDiagram
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
