<template>
  <div class="container">
    <div class="clock">{{ clock }}</div>
  </div>
</template>

<script>
export default {
  name: 'BinaryClock',
  data () {
    return {
      clock: ''
    }
  },
  methods: {
    getTime () {
      let number = (Date.now() / 1000).toString()
      this.clock = parseInt(number, 10).toString(2)
    }
  },
  mounted () {
    setInterval(this.getTime, 1000)
  }
}
</script>
<style>
  .container {
    display: flex;
    width: 100%;
    height: 100%;
    align-items: center;
  }
  .clock {
    padding: 20px;
    background: rgba(255, 255, 255, 0.5);
    margin: 0 20%;
    width: 100%;
    font-size: 3em;
    color: saddlebrown;
    font-weight: 700;
    font-family: "Roboto Mono", Arial, sans-serif;
    text-align: center;
  }
</style>
