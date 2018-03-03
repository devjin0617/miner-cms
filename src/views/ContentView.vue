<template>
  <div class="content-view">
    <el-row :gutter="20">
      <el-col :span="6">
        <miner-banner></miner-banner>
      </el-col>
      <el-col :span="6">
        <miner-banner></miner-banner>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import { MinerBanner } from '@/components'
export default {
  name: 'content-view',
  components: {
    MinerBanner
  }
}
</script>

<style>
.content-view {
  height: 100%;
}
</style>
