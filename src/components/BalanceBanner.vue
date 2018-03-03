<template>
  <div class="balance-banner">
    <div class="balance-banner-box">
      <div class="flex-item image-wrap">
        <img src="https://s2.coinmarketcap.com/static/img/coins/32x32/1.png">
      </div>
      <div style="flex:1;">
        <h2>Bitcoin (BTC)</h2>
        <p>
          1.04584938 BTC
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'balance-banner'
}
</script>

<style lang="scss" scope="scoped">
.balance-banner {
  width: 100%;
  height: 80px;
  background-color: #F2F6FC;
  border-radius: 5px;
  line-height: 10px;
  margin-top: 5px;

  .balance-banner-box {
    display:flex;
    height: 100%;
  }
}
.flex-item.image-wrap {
  width:80px;
  align-items: center;
  display: flex;
  justify-content: center;
}
</style>
