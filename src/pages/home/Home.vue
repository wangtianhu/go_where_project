<template>
    <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
    <home-hot></home-hot>
    <home-like></home-like>
    <home-weekend></home-weekend>
    </div>
</template>
<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/swiper'
import HomeIcons from './components/icons'
import HomeHot from './components/hotplace'
import HomeLike from './components/HomeLike'
import HomeWeekend from './components/HomeWeekend'
export default {
  name: 'Home',
  components:{
    HomeHeader,
    HomeSwiper,
    HomeIcons,
    HomeHot,
    HomeLike,
    HomeWeekend
  }
}
</script>
<style>
</style>

