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
  props:{
    recommendList:Array
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
