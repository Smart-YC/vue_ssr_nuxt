<template>
  <div>
    <el-menu router :default-active="this.$route.path" class="el-menu-demo" mode="horizontal" active-text-color="#fff">
      <el-menu-item index="/relation"><span slot="title">联系</span></el-menu-item>
      <el-menu-item index="/about"><span slot="title">关于</span></el-menu-item>
      <el-menu-item index="/news"><span slot="title">新闻</span></el-menu-item>
      <el-menu-item index="/product"><span slot="title">产品</span></el-menu-item>
      <el-menu-item index="/main"><span slot="title">
        <nuxt-link :to="{name:'index'}">首页</nuxt-link></span>
      </el-menu-item>
    </el-menu>
  </div>
</template>
<script>
  export default {}
</script>
<style scoped>
  a{
    text-decoration: none;
  }
  .el-menu {
    background-color: #E6E7E9;
  }

  .el-menu--horizontal > .el-menu-item:not(.is-disabled):focus, .el-menu--horizontal > .el-menu-item:not(.is-disabled):hover, .el-menu--horizontal > .el-submenu .el-submenu__title:hover {
    background-color: #E6E7E9;
  }

  .el-menu.el-menu--horizontal {
    border-bottom: none;
  }

  .el-menu.el-menu--horizontal > .el-menu-item.is-active {
    border-bottom: none;
  }

  .el-menu.el-menu--horizontal > .el-menu-item > span {
    padding: 2px 10px;
  }

  .el-menu.el-menu--horizontal > .el-menu-item.is-active > span {
    background: #000;
    padding: 2px 10px;
  }

  .el-menu--horizontal > .el-menu-item {
    float: right;
    border-bottom: none;
  }
</style>
