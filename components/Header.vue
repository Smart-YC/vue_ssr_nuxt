<template>
  <div>
    <el-menu :default-active="activeItem" class="el-menu-demo" mode="horizontal" active-text-color="#fff">
      <el-menu-item index="5"><a href="#relation">联系</a></el-menu-item>
      <el-menu-item index="4"><a href="#about">关于</a></el-menu-item>
      <el-menu-item index="3"><a href="#news">新闻</a></el-menu-item>
      <el-menu-item index="2"><a href="#product">产品</a></el-menu-item>
      <el-menu-item index="1"><a href="#main">首页</a>
      </el-menu-item>
    </el-menu>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        activeItem: '1'
      }
    }
  }
</script>
<style scoped>
  a{
    text-decoration: none;
    vertical-align: baseline;
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

  .el-menu.el-menu--horizontal > .el-menu-item > a {
    padding: 5px 20px;
  }

  .el-menu.el-menu--horizontal > .el-menu-item.is-active > a {
    background: #000;
    padding: 5px 20px;
  }

  .el-menu--horizontal > .el-menu-item {
    float: right;
    border-bottom: none;
  }
</style>
