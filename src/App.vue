<template>
  <div id="app">
    <img src="./assets/logo.png">
    <container/>
    <oneWhole/>
    <twoHalves/>
  </div>
</template>

<script>
import container from './components/container'
import oneWhole from './components/oneWhole'
import twoHalves from './components/twoHalves'

export default {
  name: 'App',
  components: {
    container,
    oneWhole,
    twoHalves
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
