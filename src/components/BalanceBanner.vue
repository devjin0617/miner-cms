<template>
  <div class="balance-banner">
    <div class="balance-banner-box">
      <div class="flex-item image-wrap">
        <img :src="imageUrl">
      </div>
      <div style="flex:1;">
        <h2>{{ name }} ({{ simbol }})</h2>
        <p>
          {{ balance }} {{ simbol }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['name', 'imageUrl', 'simbol', 'balance'],
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
