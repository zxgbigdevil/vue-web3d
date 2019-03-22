<template>
  <div class="pc-header">
    <div class="header-wrapper">
      <img src="./logo.png">
      <el-menu
        :default-active="navIndex"
        class="el-menu-nav"
        mode="horizontal"
        background-color="rgba(0,0,0,0)"
        text-color="#fff"
        active-text-color="#ffd04b"
      >
        <el-submenu index=1>
          <template slot="title">浏览模型</template>
          <el-menu-item index="1-1">文物</el-menu-item>
          <el-menu-item index="1-2">游戏</el-menu-item>
          <el-menu-item index="1-3">建筑</el-menu-item>
          <el-menu-item index="1-4">人物</el-menu-item>
          <el-menu-item index="1-5">家具</el-menu-item>
          <el-menu-item index="1-6">其它</el-menu-item>
        </el-submenu>
        <el-menu-item index="2">操作教程</el-menu-item>
        <el-menu-item index="3">社区互动</el-menu-item>
        <el-menu-item index="4">联系我们</el-menu-item>
      </el-menu>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navIndex: '1'
    }
  }
}
</script>

<style lang="scss" scoped type="text/scss">
  @import "~common/scss/variable.scss";

  .pc-header {
    width: 100%;
    height: 70px;
    background: $header-background;
    .header-wrapper {
      width: $min-width;
      margin: auto;
      display: flex;
      align-items: center;
      > img {
        width: 200px;
        height: 50px;
      }
      .el-menu-nav {
        height: 70px;
      }
    }
  }
</style>
