<template>
  <div>
    <home-header :city="city"></home-header>
    <home-swiper :swiperList="swiperList"></home-swiper>
    <home-icons :iconsList="iconsList"></home-icons>
    <home-recommend :recommendList="recommendList"></home-recommend>
  </div>
</template>
<script>
import homeHeader from './compenents/header'
import homeSwiper from './compenents/swiper'
import homeIcons from './compenents/icons'
import homeRecommend from './compenents/recommend'
import axios from 'axios'

export default {
  name: 'home',
  data(){
    return{
      city:'',
      swiperList:[],
      iconsList:[],
      recommendList:[]
    }
  },
  components: {
    homeHeader,
    homeSwiper,
    homeIcons,
    homeRecommend
  },
  methods: {
    getHomeInfo() {
      axios.get('/api/index.json')
        .then(this.getHomeInfoSucc)
    },
    getHomeInfoSucc(res) {
      console.log(res)
      res=res.data
      if(res.ret&&res.data){
        const data=res.data
        this.city=data.city,
          this.swiperList=data.swiperList,
          this.iconsList=data.iconsList,
          this.recommendList=data.recommendList

      }

    }
  },
  mounted() {
    this.getHomeInfo()
  }
}
</script>
<style>

</style>
