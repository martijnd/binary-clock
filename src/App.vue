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
  body {
    background: #fff url("./assets/bg.png") repeat;
    background-size: 60px;
    width: 100vw;
    height: 100vh;
  }

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  height: 100%;
}
</style>
