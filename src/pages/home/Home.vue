<template>
    <div>
    <home-header></home-header>
    <home-swiper :list="swiperList"></home-swiper>
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
import axios from 'axios'
export default {
  name: 'Home',
  data () {
    return {
      swiperList:[]
    }
  },
  components:{
    HomeHeader,
    HomeSwiper,
    HomeIcons,
    HomeHot,
    HomeLike,
    HomeWeekend
  },
  methods:{
    getIndexInfo(){
      console.log(1111);
      
      axios.get('/api/index.json')
      .then(this.getIndexData)
    },
    getIndexData(res){
      
      const  data = res.data.data;
      this.swiperList = data.swiperList;
      console.log(data);
    }
  },
  mounted(){
    this.getIndexInfo()
  }
}
</script>
<style>
</style>

