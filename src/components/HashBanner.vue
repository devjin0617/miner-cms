<template>
  <div class="hash-banner">
    <div class="hash-banner-box">
      <div class="flex-item image-wrap">
        <img :src="imageUrl">
      </div>
      <div style="flex:1;">
        <h2>{{ name }} ({{ simbol }})</h2>
        <p>
          {{ hashValue }} TH/s
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['name', 'imageUrl', 'simbol', 'hashValue'],
  name: 'hash-banner'
}
</script>

<style lang="scss" scope="scoped">
.hash-banner {
  width: 100%;
  height: 80px;
  background-color: #F2F6FC;
  border-radius: 5px;
  line-height: 10px;
  margin-top: 5px;

  .hash-banner-box {
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
