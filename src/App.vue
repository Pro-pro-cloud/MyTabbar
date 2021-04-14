<template>
  <div id="app">
    <tabbar>
      <TabbarItem>
        <img slot="item-icon" src="./assets/img/tabbar/home.svg" alt="">
        <div slot="item-text">首页</div>
      </TabbarItem>
      <TabbarItem>
        <img slot="item-icon" src="./assets/img/tabbar/category.svg" alt="">
        <div slot="item-text">分类</div>
      </TabbarItem>
      <TabbarItem>
        <img slot="item-icon" src="./assets/img/tabbar/shopcart.svg" alt="">
        <div slot="item-text">购物车</div>
      </TabbarItem>
      <TabbarItem>
        <img slot="item-icon" src="./assets/img/tabbar/profile.svg" alt="">
        <div slot="item-text">我的</div>
      </TabbarItem>
    </tabbar>
  </div>
</template>

<script>
import Tabbar from './components/tabbar/Tabbar'
import TabbarItem from './components/tabbar/TabbarItem'

export default {
  name: 'App',
  components: {
    Tabbar,
    TabbarItem
  }
}
</script>

<style lang="scss">
@import "./assets/css/base.css";

</style>
