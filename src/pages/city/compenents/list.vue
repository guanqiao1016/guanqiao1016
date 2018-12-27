<template>
    <div class="list" ref="wrapper">
      <div>
      <div class="area">
        <div class="title border-topbottom">当前城市</div>
        <div class="button-list">
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">热门城市</div>
        <div class="button-list">
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
          <div class="button-wraper">
            <div class="button">济南</div>
          </div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">A</div>
        <div class="item-list">
          <div class="item border-bottom">澳门</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">澳门</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">澳门</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">澳门</div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">B</div>
        <div class="item-list">
          <div class="item border-bottom">北京</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">北京</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">北京</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">北京</div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">C</div>
        <div class="item-list">
          <div class="item border-bottom">成都</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">成都</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">成都</div>
        </div>
        <div class="item-list">
          <div class="item border-bottom">成都</div>
        </div>
      </div>
      </div>
    </div>
</template>
<script>
import BScroll from 'better-scroll'
export default {
   name: 'cityList',
  mounted(){
    this.scroll = new BScroll(this.$refs.wrapper)
  }
}
</script>
<style lang="stylus" scoped>
    .border-topbottom
       &:before
         border-color:#ccc
       &:after
         border-color:#ccc
    .border-bottom
       &:before
        border-color:#ccc
    .list
       position:absolute
       top:1.58rem
       left:0
       right:0
       bottom:0
       overflow:hidden
      .title
         background:#eee
         line-height:.54rem
         padding-left:.2rem
         color:#666
      .button-list
        padding:.1rem .6rem .1rem .1rem
        overflow:hidden
        .button-wraper
           float:left
           width:33%
          .button
            padding:.1rem 0
            margin:.15rem
            text-align:center
            border:solid .02rem #ccc
            border-radius:.05rem
      .item-list
        .item
          margin-left:.2rem
          line-height:.66rem
          color:#333
          padding.1rem

</style>
