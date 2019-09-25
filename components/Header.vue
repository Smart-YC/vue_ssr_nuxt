<template>
  <div>
    <el-menu :default-active="activeItem" class="el-menu-demo" mode="horizontal" active-text-color="#fff">
      <el-menu-item index="5"><span slot="title"><a href="#relation">联系</a></span></el-menu-item>
      <el-menu-item index="4"><span slot="title"><a href="#about">关于</a></span></el-menu-item>
      <el-menu-item index="3"><span slot="title"><a href="#news">新闻</a></span></el-menu-item>
      <el-menu-item index="2"><span slot="title"><a href="#product">产品</a></span></el-menu-item>
      <el-menu-item index="1"><span slot="title"><a href="#main">首页</a></span>
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
