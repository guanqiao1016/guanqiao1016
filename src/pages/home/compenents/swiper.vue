<template>
  <div class="wapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id" ><img  class="swiper-img" :src="item.imgUrl"/></swiper-slide>
      <swiper-slide ><img  class="swiper-img" src=""/></swiper-slide>
      <swiper-slide ><img  class="swiper-img" src=""/></swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>

</template>
<script>
export default {
  name: 'homeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination'
      },
      swiperList: [{id: '0001',
        imgUrl: 'http://img1.qunarzz.com/vc/a4/29/dd/4a0734b77f675da2a8ca4a9879.jpg'}, {id: '0002',
        imgUrl: 'http://img1.qunarzz.com/vc/d4/d0/62/a6b7c23c1b251dfc874ce66efa.jpg'}, {id: '0003',
        imgUrl: 'http://img1.qunarzz.com/vc/f5/10/9c/b647d3ee724a720ce0fa6101f0.jpg'}
      ]
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
