<template>
<div class="icons">
  <swiper>
    <swiper-slide v-for="(page,index) of pages" :key="index">
        <div class="icon" v-for='item of page' :key='item.id'>
            <div class="icon-img">
             <img  class="icon-img-cont" :src='item.imgUrl' >
            </div>
            <p class="icon-des">{{item.test}}</p>
          </div>
    </swiper-slide>
  </swiper>
</div>
</template>
<script>
export default {
  name: 'homeIcons',
  data () {
    return {
      iconsList: [{
        id : '001',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
        test: '景点门票'},
        {
          id : '002',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
          test: '济南必游'},
        {
          id : '003',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/96/c70f1e85ae4a4f02.png',
          test: '自然风光'},
        {
          id : '004',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/20/831d62d2e1c7be02.png',
          test: '趵突泉'},
        {id : '005',
      imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
      test: '景点门票'},
    {
      id : '006',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
      test: '济南必游'},
    {
      id : '007',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/96/c70f1e85ae4a4f02.png',
      test: '自然风光'},
    {
      id : '008',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/20/831d62d2e1c7be02.png',
      test: '趵突泉'},
        {id : '009',
      imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
      test: '景点门票'},
{
  id : '010',
    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
  test: '济南必游'},
{
  id : '011',
    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/96/c70f1e85ae4a4f02.png',
  test: '自然风光'},
{
  id : '012',
    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/20/831d62d2e1c7be02.png',
  test: '趵突泉'}
      ]
    }
},
  computed:{
    pages (){
      const pages=[]
      this.iconsList.forEach((item,index) =>{
        const page = Math.floor(index/8)
        if(!pages[page]){
          pages[page]=[]
        }
        pages[page].push(item)
      })
      return pages

    }
  }
}
</script>
<style lang="stylus" scoped>
    .icons >>> .swiper-container
          overflow:hidden
          height: 0
          padding-bottom:50%
    .icon
       position:relative
       overflow:hidden
       float:left
       width:25%
       height:0
       padding-bottom:25%
      .icon-img
           position:absolute
           top:0
           left:0
           right:0
           bottom:.44rem
           overflow:hidden
           box-sizing:border-box
           padding:.1rem
        .icon-img-cont
           width:100%
           display:block
           margin:0 auto
      .icon-des
        position:absolute
        bottom:0
        left:0
        right:0
        height:.44rem
        line-height:.44rem
        text-align:center
        color:#333
</style>
