<template>
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
</template>
<script>
    export default {
        name: 'cityList'
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
  .title
     background:#eee
     line-height:.4rem
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
