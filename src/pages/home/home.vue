<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
    <home-recommend></home-recommend>
  </div>
</template>
<script>
import homeHeader from './compenents/header'
import homeSwiper from './compenents/swiper'
import homeIcons from './compenents/icons'
import homeRecommend from './compenents/recommend'

export default {
  name: 'home',
  components: {
    homeHeader,
    homeSwiper,
    homeIcons,
    homeRecommend
  }
}
</script>
<style>

</style>
