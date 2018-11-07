<template>
  <div class="page-warpper">
    <div class="nav">
      <Nav></Nav>
    </div>
    <div class="content">
      <h1>{{ msg }}</h1>
    </div>
    <div class="footer">
      <Foot-content></Foot-content>
    </div>
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
