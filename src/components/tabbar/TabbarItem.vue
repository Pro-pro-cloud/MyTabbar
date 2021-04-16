<template>
<div class="tab-bar-item" @click="itemClick">
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
  props: {
    path: String
  },
  data () {
    return {
      isActive: false
    }
  },
  methods: {
    itemClick () {
      this.$router.replace(this.path).catch(err => err)
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
