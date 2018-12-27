<template>
  <div>
    <city-header></city-header>
    <city-search></city-search>
    <city-list></city-list>
    <city-alphabet></city-alphabet>
  </div>
</template>
<script>
import cityHeader from './compenents/header'
import citySearch from './compenents/search'
import cityList from './compenents/list'
import cityAlphabet from './compenents/alphabet'
export default {
  name: 'city',
  components:{
    cityHeader,
    citySearch,
    cityList,
    cityAlphabet
  }
}
</script>
<style lang="stylus">

</style>
