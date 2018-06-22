<template>
   <div class="wrapper">
        <swiper :options="swiperOption">
    <!-- slides -->
    <swiper-slide v-for="(item,index) in srcImg" :key="index">
        <img class="swiper-img" :src="item" alt="">
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    <div class="swiper-scrollbar"   slot="scrollbar"></div>
  </swiper>
   </div>
</template>
 <script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOption: {
          pagination:'.swiper-pagination',
          loop:true
      },
      srcImg: [
        "http://img1.qunarzz.com/piao/fusion/1805/3b/ef86879aa50e3002.jpg_750x200_2a108508.jpg",
        "http://img1.qunarzz.com/piao/fusion/1806/64/cc63aa526e8bb302.png_750x200_d32776c5.png",
        "http://img1.qunarzz.com/piao/fusion/1806/66/d0c77dd556488b02.jpg_750x200_7c908215.jpg",
        "http://img1.qunarzz.com/piao/fusion/1805/13/6332699c44387902.jpg_750x200_b7afa4f8.jpg"
      ]
    };
  },
  mouted(){
      this.swiper.slideTo(4, 1000, false)
  }
};
</script>
 <style lang="scss" scoped>
.wrapper {
    overflow: hidden;
    width: 100%;
    height: 0;
    padding-bottom: 31.25%;
  .swiper-img {
    width: 100%;
  }
  .swiper-pagination>span{
      background-color: #fff;
  }
}

</style>
 