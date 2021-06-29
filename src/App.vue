<template>
  <div id="app">
    <router-view></router-view>
    <Tar>
    <tarBarItem path="/home">
      <img slot="item-icon" src="./assets/img/tabbar/home.svg">
      <img slot="item-icon-active" src="./assets/img/tabbar/home-active.svg">
      <div slot="item-text">首页</div>
    </tarBarItem>
    <tarBarItem path="/category">
      <img slot="item-icon" src="./assets/img/tabbar/category.svg">
      <img slot="item-icon-active" src="./assets/img/tabbar/category-active.svg">
      <div slot="item-text">分类</div>
    </tarBarItem>
    <tarBarItem path="/cart">
      <img slot="item-icon" src="./assets/img/tabbar/cart.svg">
      <img slot="item-icon-active" src="./assets/img/tabbar/cart-active.svg">
      <div slot="item-text">购物车</div>
    </tarBarItem>
    <tarBarItem path="/Profile">
      <img slot="item-icon" src="./assets/img/tabbar/mine.svg">
      <img slot="item-icon-active" src="./assets/img/tabbar/mine-active.svg">
      <div slot="item-text">我的</div>
    </tarBarItem>
  </Tar>
  </div>
</template>

<script>
  import Tar from './components/tabber/tabber'
  import tarBarItem from './components/tabber/tarBarItem'
export default {
  name: 'App',
  components: {
    Tar,
    tarBarItem
  }
}
</script>

<style>
  @import "./assets/css/base.css";

</style>
