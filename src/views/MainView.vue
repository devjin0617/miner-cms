<template>
  <div>
    <el-container class="el-container-main">
      <el-header>
        <top-view></top-view>
      </el-header>
      <el-container>
        <el-aside width="200px">
          <side-view></side-view>
        </el-aside>
        <el-main>
          <content-view></content-view>
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import TopView from '@/views/TopView'
import SideView from '@/views/SideView'
import ContentView from '@/views/ContentView'
export default {
  name: 'main-view',
  components: {
    TopView,
    SideView,
    ContentView
  }
}
</script>
