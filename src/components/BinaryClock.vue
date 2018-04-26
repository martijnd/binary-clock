<template>
  <div class="hello">
    {{ clock }}
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      clock: ''
    }
  },
  methods: {
    getTime () {
      let bin = ''
      let number = (Date.now() / 1000).toString()
      this.clock = parseInt(number, 10).toString(2)
    }
  },
  mounted () {
    setInterval(this.getTime, 1000)
  }
}
</script>
