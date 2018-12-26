<template>
  <div>
    <city-header></city-header>
    <city-search></city-search>
    <city-list></city-list>
  </div>
</template>
<script>
import cityHeader from './compenents/header'
import citySearch from './compenents/search'
import cityList from './compenents/list'
export default {
  name: 'city',
  components:{
    cityHeader,
    citySearch,
    cityList
  }
}
</script>
<style lang="stylus">

</style>
