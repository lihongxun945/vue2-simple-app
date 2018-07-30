<template>
  <div class="hello">
    <h1>{{ upperMsg}}</h1>
    <h2>Essential Links</h2>
    <p>{{ doubleMsg }}</p>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  computed: {
    upperMsg () {
      return this.msg.toUpperCase()
    },
    doubleMsg () {
      return this.msg + this.msg
    }
  },
  mounted () {
    this.msg = 'aaaa'
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
</style>
