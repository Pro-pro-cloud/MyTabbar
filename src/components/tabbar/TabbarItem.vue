<template>
<div class="tab-bar-item">
  <div v-if="!isActive"><slot  name="item-icon"></slot></div>
  <div v-else><slot  name="item-icon-active"></slot></div>
  <div :class="{active : isActive}"><slot name="item-text"></slot></div>
  <!-- <img src="../../assets/img/tabbar/home.svg" alt="">
  <div>首页</div> -->
</div>
</template>

<script>
export default {
  name: 'TabbarItem',
  data () {
    return {
      isActive: false
    }
  }
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

.active {
  color: red;
}
</style>
