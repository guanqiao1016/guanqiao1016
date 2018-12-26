<template>
  <div class="wapper">
    <swiper :options="swiperOption" v-if="swiperList.length">
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id" >
        <img  class="swiper-img" :src="item.imgUrl"/>
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>

</template>
<script>
export default {
  name: 'homeSwiper',
  props:{
    swiperList:Array
  },
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop:true,
        speed: 2000,
        autoplay:5000
      }
    }
  }
}
</script>
<style lang="stylus" scoped>
  .wapper >>> .swiper-pagination-bullet-active
      background : #fff !important
  .wapper
     width:100%
     height:0
     overflow:hidden
     padding-bottom:31.25%
     .swiper-img
       width:100%
</style>
