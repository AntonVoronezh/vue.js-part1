<template lang="pug">
div

  h3.jjjjj tt
  innerComp(
    placeholder="ff2ff gggggg"
  )
</template>

<script>
import inner from './components/inner'

export default {
  name: 'app',
  components:{
    innerComp: inner
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="scss" scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
.jjjjj {
  color: red;
}
</style>
