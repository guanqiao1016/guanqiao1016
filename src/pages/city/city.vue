<template>
  <div>
    <city-header></city-header>
    <city-search></city-search>
  </div>
</template>
<script>
import cityHeader from './compenents/header'
import citySearch from './compenents/search'
export default {
  name: 'city',
  components:{
    cityHeader,
    citySearch
  }
}
</script>
<style lang="stylus">

</style>
