<template>
  <div>
    <el-row :gutter="20">
      <el-col v-for="(item, index) in minerList" :span="6" :key="index">
        <miner-banner :title="item.title" :text="item.text"></miner-banner>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import { MinerBanner } from '@/components'
export default {
  name: 'dashboard',
  data () {
    return {
      minerList: [
        {
          title: 'P106',
          text: '4 MINER (24 WAY)'
        },
        {
          title: 'ASIC S9',
          text: '1 MINER'
        },
        {
          title: 'ASIC L3+',
          text: '1 MINER'
        },
        {
          title: 'ASIC D3',
          text: '1 MINER'
        }
      ]
    }
  },
  components: {
    MinerBanner
  }
}
</script>

<style>

</style>
