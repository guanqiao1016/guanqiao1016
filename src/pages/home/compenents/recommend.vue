<template>
<div class="recommend">
  <div class="title">猜你喜欢</div>
  <ul>
  <li class="content border-bottom" v-for="item of recommendList" :key="item.id">
    <div class="img-img">
        <img class="img" :src="item.imgUrl">
    </div>
    <div class="info">
      <p class="img-title">{{item.title}}</p>
      <p class="img-com">{{item.com}}条评论</p>
    </div>
  </li>
  </ul>
</div>
</template>
<script>
export default {
  name : 'homeRecommend',
  data() {
    return { recommendList: [
        {id: '0001', imgUrl: 'http://img1.qunarzz.com/sight/p0/1705/e9/e993699e058a65a6a3.water.jpg_200x200_64b651df.jpg', title:'世贸宽厚里',com:'1178'},
        {id: '0002', imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/da/da7c46e2eef8714e.water.jpg_200x200_2a340470.jpg',title:'千佛山',com:'2020'},
        {id: '0003', imgUrl: 'http://img1.qunarzz.com/sight/p0/1606/23/237ad24ea960b2f290.water.jpg_200x200_5c711497.jpg',title:'趵突泉公园',com:'15327'},
        {id: '0003', imgUrl: 'http://img1.qunarzz.com/sight/p0/1610/f9/f90e75166d28d4a9a3.img.jpg_200x200_d7f84fbf.jpg',title:'红叶谷生态文化旅游区',com:'13327'}
      ]

    }
  }
}
</script>
<style lang="stylus" scoped>
  .recommend
     margin:.2rem 0
    .title
      height:.6rem
      line-height:.6rem
      font-size:.3rem
      text-indent:.2rem
      background:#eee
    .content
      height:0
      width:100%
      padding-bottom:27%
      overflow:hidden
      display:flex
      .img-img
          width:2rem
          height:2rem
          overflow:hidden
          padding:.1rem
         .img
           width:100%
      .info
        padding:.1rem
        flex:1
        .img-title
          font-size:.4rem
          line-height:1rem
        .img-com
          font-size:.3rem
          line-height:.5rem
          color:#aaa
</style>
