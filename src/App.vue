<template>
  <div id="app">
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
    <main-tab-bar></main-tab-bar>
  </div>
</template>


<script>
import MainTabBar from 'components/connection/mainTabBar/MainTabBar'

export default{
  name:'app', 
  components:{
    MainTabBar
  }
}
</script>

<style>
  @import "assets/css/base.css"
</style>
