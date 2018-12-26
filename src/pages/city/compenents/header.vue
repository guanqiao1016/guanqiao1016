<template>
  <div class="header">
      <router-link to="/">
      <div class="iconfont icon-back">&#xe624;</div>
        </router-link>
      城市选择
  </div>

</template>
<script>
export default {
  name:'cityHeader'
}
</script>
<style lang="stylus" scoped>
  @import '~styles/varibles.styl';
  .header
     position:relative
     overflow:hidden
     line-height:.86rem
     font-size:.4rem
     color:#fff
     background:$bgColor
     text-align:center
     .icon-back
       position:absolute
       top:0
       left:.18rem
       bottom:0
       color:#fff

</style>
