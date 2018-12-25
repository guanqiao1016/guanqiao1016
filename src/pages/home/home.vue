<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
  </div>
</template>
<script>
import homeHeader from './compenents/header'
import homeSwiper from './compenents/swiper'
import homeIcons from './compenents/icons'

export default {
  name: 'home',
  components: {
    homeHeader,
    homeSwiper,
    homeIcons
  }
}
</script>
<style>

</style>
