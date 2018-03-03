<template>
  <div>
    <div>
      <h2>Miner List</h2>
      <el-row :gutter="20">
        <el-col v-for="(item, index) in minerList" :span="6" :key="index">
          <miner-banner :title="item.title" :text="item.text"></miner-banner>
        </el-col>
      </el-row>
    </div>
    <div class="top-margin"></div>
    <el-row :gutter="20">
      <el-col :span="6">
        <h2>Balance</h2>
        <balance-banner v-for="(item, index) in balanceList" :key="index"
          :name="item.name"
          :simbol="item.simbol"
          :image-url="item.imageUrl"
          :balance="item.balance"
        ></balance-banner>
      </el-col>
      <el-col :span="6">
        <h2>Miner Hashrate</h2>
        <hash-banner v-for="(item, index) in hashList" :key="index"
          :name="item.name"
          :simbol="item.simbol"
          :image-url="item.imageUrl"
          :hashValue="item.value"
        ></hash-banner>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import { MinerBanner, BalanceBanner, HashBanner } from '@/components'
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
      ],
      balanceList: [
        {
          name: 'Bitcoin',
          simbol: 'BTC',
          imageUrl: 'https://s2.coinmarketcap.com/static/img/coins/32x32/1.png',
          balance: '1.04857395'
        },
        {
          name: 'Ethereum',
          simbol: 'ETH',
          imageUrl: 'https://s2.coinmarketcap.com/static/img/coins/32x32/1027.png',
          balance: '38.486934'
        },
        {
          name: 'ZenCash',
          simbol: 'ZEN',
          imageUrl: 'https://s2.coinmarketcap.com/static/img/coins/32x32/1698.png',
          balance: '27.839'
        }
      ],
      hashList: [
        {
          name: 'Bitcoin',
          simbol: 'BTC',
          imageUrl: 'https://s2.coinmarketcap.com/static/img/coins/32x32/1.png',
          value: '13.5'
        },
        {
          name: 'Ethereum',
          simbol: 'ETH',
          imageUrl: 'https://s2.coinmarketcap.com/static/img/coins/32x32/1027.png',
          value: '120'
        },
        {
          name: 'ZenCash',
          simbol: 'ZEN',
          imageUrl: 'https://s2.coinmarketcap.com/static/img/coins/32x32/1698.png',
          value: '6.04'
        }
      ]
    }
  },
  components: {
    MinerBanner,
    BalanceBanner,
    HashBanner
  }
}
</script>

<style>
.top-margin {
  margin-top: 20px;
}
</style>
