<template>
  <h1 class="logo">测试 vueUse 的鼠标坐标</h1>
  <h3>Mouse: {{ x }} x {{ y }}</h3>
  <el-row class="mb-4">
    <el-button disabled>Default</el-button>
    <el-button type="primary">Primary</el-button>
    <el-button type="success">Success</el-button>
    <el-button type="info">Info</el-button>
    <el-button type="warning">Warning</el-button>
    <el-button type="danger">Danger</el-button>
  </el-row>

  <el-row>
    <el-button plain disabled>Plain</el-button>
    <el-button type="primary" plain disabled>Primary</el-button>
    <el-button type="success" plain disabled>Success</el-button>
    <el-button type="info" plain disabled>Info</el-button>
    <el-button type="warning" plain disabled>Warning</el-button>
    <el-button type="danger" plain disabled>Danger</el-button>
  </el-row>
</template>

<script lang="ts" setup>
import { useMouse } from '@vueuse/core'

const { x, y } = useMouse()
</script>

<style lang="scss">
.logo {
  background-color: red;
}
</style>
