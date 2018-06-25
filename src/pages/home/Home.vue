<template>
    <div>
    <home-header></home-header>
    <home-swiper :list="swiperList"></home-swiper>
    <home-icons :list="iconsList"></home-icons>
    <home-hot :list="recommendList"></home-hot>
    <home-like :list="recommendList"></home-like>
    <home-weekend :list="weekendList"></home-weekend>
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
      swiperList:[],
      iconsList:[],
      recommendList:[],
      weekendList:[]
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
      this.iconsList = data.iconList;
      this.recommendList = data.recommendList;
      this.weekendList = data.weekendList;
      console.log( this.weekendList);
    }
  },
  mounted(){
    this.getIndexInfo()
  }
}
</script>
<style>
</style>

