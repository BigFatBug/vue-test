<template>
  <div>
    <el-header>
      <img class="logo" src="../assets/img/logo.png"/>
      <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal">
        <el-menu-item index="1">主页</el-menu-item>
        <el-menu-item index="2">个人中心</el-menu-item>
        <el-menu-item index="3">课程中心</el-menu-item>
      </el-menu>
    </el-header>
  </div>
</template>
<style>
  .logo{
    position: relative;
    margin-left: 5%;
    margin-right: 5%;
    float: left;
    z-index: 999;
  }
  .el-menu{;
    active-text-color: #00d1b2;
  }
  .el-menu-item{
    font-size: 25px;
  }
  .el-menu--horizontal>.el-menu-item.is-active, .el-menu--horizontal>.el-submenu.is-active .el-submenu__title{
    border-bottom: 0px;
  }
</style>
<script>
  export default {
    name: "homeHeader",
    data() {
      return {
        activeIndex: '1'
      };
    },
  }
</script>
