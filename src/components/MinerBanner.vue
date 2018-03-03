<template>
  <div class="miner-banner">
    <div class="minder-banner-box">
      <h1>{{ title }}</h1>
      <p>{{ text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'miner-banner',
  props: ['title', 'text']
}
</script>

<style lang="scss" scope="scoped">
.miner-banner {
  width: 100%;
  height: 110px;
  background-color: #409EFF;
  color: white;
  border-radius: 5px;
  line-height: normal;

  .minder-banner-box {
    padding: 5px 20px;
  }
}
</style>
