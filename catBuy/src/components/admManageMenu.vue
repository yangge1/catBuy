<template>
  <div class="menu-page">
    <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" background-color="#324057"
      text-color="#fff" active-text-color="#ffd04b" >
      <el-menu-item index="1">
        <i class="el-icon-menu"></i>
        <span slot="title">首页</span>
      </el-menu-item>
      <el-submenu index="2">
        <template slot="title">
          <i class="el-icon-document"></i>
          <span>系统管理</span>
        </template>
        <el-menu-item index="1-1">用户列表</el-menu-item>
          <el-menu-item index="1-2">产品列表</el-menu-item>
          <el-menu-item index="1-3">订单列表</el-menu-item>
          <el-menu-item index="1-4">管理员列表</el-menu-item>
          <el-menu-item index="1-5">活动管理</el-menu-item>
          <el-menu-item index="1-6">菜单管理</el-menu-item>
          <el-menu-item index="1-7">轮播图管理</el-menu-item>
      </el-submenu>
      <el-submenu index="3">
        <template slot="title">
          <i class="el-icon-plus"></i>
          <span slot="title">添加数据</span>
        </template>
        <el-menu-item index="3-1">添加商品</el-menu-item>
          <el-menu-item index="3-2">添加菜单</el-menu-item>
      </el-submenu>
      <el-submenu index="4">

        <template slot="title">
          <i class="el-icon-star-on"></i>
          <span slot="title">图表</span>
        </template>
        <el-menu-item index="4-1">用户分布</el-menu-item>
      </el-submenu>
      <el-submenu index="5">

        <template slot="title">
          <i class="el-icon-setting"></i>
          <span slot="title">设置</span>
        </template>
        <el-menu-item index="5-1">管理员设置</el-menu-item>
      </el-submenu>
      <el-submenu index="6">

        <template slot="title">
          <i class="el-icon-warning"></i>
          <span slot="title">说明</span>
        </template>
         <el-menu-item index="6-1">说明</el-menu-item>
      </el-submenu>
    </el-menu>
      
  </div>
</template>
<script>
  export default {
    methods: {
      handleOpen(key, keyPath) {
        console.log(key, keyPath);
      },
      handleClose(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }

</script>
<style lang="less">
  .menu-page {
    height: 100%;
    .el-menu{
      height: 100%;
      .el-submenu{
         .el-menu-item{
           background: #1f2d3d!important;
         }
      }
    }
  }

</style>
