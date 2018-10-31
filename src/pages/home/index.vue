<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <el-input-number v-model="num1"
                     @change="handleChange"
                     :min="1"
                     :max="10"
                     label="描述文字"></el-input-number>
    <h2>hello world</h2>
  </div>
</template>

<script>
import { InputNumber } from 'element-ui'

export default {
  name: 'Home',
  components: {
    InputNumber
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
