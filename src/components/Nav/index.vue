<template>
  <div class="nav">
    <div class="nav1">
      nav1
      <div class="nav2">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Nav',
  data () {
    return {
      msg: '这个是nav！'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.nav {
  background-image: url(https://upload-images.jianshu.io/upload_images/26865-13409e03aa025ca6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240);
}
</style>

<style lang="less" scoped>
.nav {
  // background-image: url(https://upload-images.jianshu.io/upload_images/26865-13409e03aa025ca6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240);
  background: red;
  .nav1 {
    background: black;
    .nav2 {
      background: blue;
    }
  }
}
</style>
