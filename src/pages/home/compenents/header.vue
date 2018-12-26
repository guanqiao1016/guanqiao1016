<template>
<div class="header">
  <div class="header-left">
    <span class="iconfont">&#xe624;</span>
  </div>
  <div class="header-input">
    <span class="iconfont">&#xe632;</span>
    输出城市\景点\游玩主题</div>
  <div class="header-right">{{this.city}} <span class="iconfont">&#xe615;</span>
  </div>
</div>
</template>
<script>
export default {
  name: 'homeHeader',
  props: {
    city:String
  }
}
</script>
<style lang="stylus" type="text/stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display: flex
    line-height:.86rem
    background: $bgColor
    color: #fff

  .header-left
    width: .64rem
    float: left
    text-align center
  .header-input
    flex:1
    background: #fff
    color: #ccc
    height: .64rem
    line-height  .64rem
    border-radius:.1rem
    margin: .12rem
    padding-left:.2rem
  .header-right
    width:1.24rem
    float: right
    text-align center
    padding-right:.2rem
</style>
