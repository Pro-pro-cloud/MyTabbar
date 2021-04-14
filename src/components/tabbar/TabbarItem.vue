<template>
<div class="tab-bar-item">
  <slot name="item-icon"></slot>
  <slot name="item-text"></slot>
  <!-- <img src="../../assets/img/tabbar/home.svg" alt="">
  <div>首页</div> -->
</div>
</template>

<script>
export default {
  name: 'TabbarItem'
}
</script>

<style>
.tab-bar-item {
  flex: 1;
  text-align: center;
  height: 49px;
  /* line-height: 49px; */
}
.tab-bar-item img {
  width: 24px;
  height: 24px;
  margin-top: 3px;
  margin-bottom: 2px;
  font-size: 14px;
  vertical-align: middle;
}
</style>
