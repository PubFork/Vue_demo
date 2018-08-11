<template>
  <div id="app" @touchmove.prevent>
    <!-- 使用组件 -->
    <m-header></m-header>
    <tab></tab>
    <!-- 包裹可以不用再次请求，直接进入到缓存中 -->
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
    <player></player>
  </div>
</template>

<script type="text/ecmascript-6">
  // 引入
  import MHeader from 'components/m-header/m-header'
  import Tab from 'components/tab/tab'
  import Player from 'components/player/player'
  // 注册组件
  export default {
    components: {
      MHeader,
      Tab,
      Player
    }
  }
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
</style>
