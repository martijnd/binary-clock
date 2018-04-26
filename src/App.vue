<template>
  <div id="app">
    <BinaryClock/>
  </div>
</template>

<script>
import BinaryClock from './components/BinaryClock'

export default {
  name: 'App',
  components: {
    BinaryClock
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
