<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
  </div>
</template>
<script>
import homeHeader from './compenents/header'
import homeSwiper from './compenents/swiper'
export default {
  name: 'home',
  components: {
    homeHeader,
    homeSwiper
  }
}
</script>
<style>

</style>
