<template>
  <div class="menu-page">
    <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" background-color="#545c64"
      text-color="#fff" active-text-color="#ffd04b">
      <el-menu-item index="1">
        <i class="el-icon-menu"></i>
        <span slot="title">首页</span>
      </el-menu-item>
      <el-submenu index="2">
        <template slot="title">
          <i class="el-icon-location"></i>
          <span>系统管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="1-1">用户列表</el-menu-item>
          <el-menu-item index="1-2">产品列表</el-menu-item>
          <el-menu-item index="1-3">订单列表</el-menu-item>
          <el-menu-item index="1-4">管理员列表</el-menu-item>
          <el-menu-item index="1-5">活动管理</el-menu-item>
          <el-menu-item index="1-6">菜单管理</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-menu-item index="3">
        <template slot="title">
          <i class="el-icon-plus"></i>
          <span slot="title">添加数据</span>
        </template>
        <el-menu-item-group>

          <el-menu-item index="1-1">添加商品</el-menu-item>
          <el-menu-item index="1-2">添加菜单</el-menu-item>
        </el-menu-item-group>
      </el-menu-item>
      <el-menu-item index="3" disabled>
        
        <template slot="title">
          <i class="el-icon-star-on"></i>
        <span slot="title">图表</span>
        </template>
        <el-menu-item-group>

          <el-menu-item index="1-1">用户分布</el-menu-item>
        </el-menu-item-group>
      </el-menu-item>

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
  }

</style>
