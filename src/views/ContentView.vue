<template>
  <div class="content-view">
    <dashboard></dashboard>
  </div>
</template>

<script>
import Dashboard from './contents/Dashboard'
export default {
  name: 'content-view',
  components: {
    Dashboard
  }
}
</script>

<style>
.content-view {
  height: 100%;
}
</style>
