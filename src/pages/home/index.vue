<template>
  <div class="hello">
    <Nav></Nav>
    <h1>{{ msg }}</h1>
    <Foot-content></Foot-content>
  </div>
</template>

<script>
import Nav from '../../components/Nav/index'
import FootContent from '../../components/FootContent/index'
export default {
  name: 'Home',
  components: {
    Nav,
    FootContent
  },
  data () {
    return {
      msg: '这个是home/index页面',
      num1: 1
    }
  },
  methods: {
    handleChange (value) {
      console.log(value)
    }
  }
}
</script>

<style scoped>
h1,
h2 {
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
