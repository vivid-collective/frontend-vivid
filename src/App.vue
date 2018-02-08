<template>
  <div id="app">
        <el-row>
      <el-col :span="24">
        <el-menu theme="dark" default-active="1" class="el-menu-demo" mode="horizontal">
          <el-menu-item index="1">Processing Center</el-menu-item>
          <el-submenu index="2">
            <template slot="title">Workspace</template>
            <el-menu-item index="2-1">item one</el-menu-item>
          </el-submenu>
          <el-menu-item index="3">Orders</el-menu-item>
        </el-menu>
      </el-col>
    </el-row>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>

</style>
