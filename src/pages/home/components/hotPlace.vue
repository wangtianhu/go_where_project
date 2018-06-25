<template>
   <div class="hotp">
       <div class="recommendtitle clearfix">
           <div class="recommend-left">
               <img src="http://img1.qunarzz.com/piao/fusion/1711/16/bfbb9874e8f11402.png" alt="">
               <span>本周热门推荐</span>
           </div>
           <div class="recommend-right">
               <span>全部榜单</span>
               <span class="iconfont icon-back"></span>
           </div>
       </div>
        <div class="wrapper">
        <swiper :options="swiperOption">
    <!-- slides -->
    <swiper-slide class="hotSwiper" v-for="(item,index) in list" :key="index">
        <img class="swiper-img" :src="item.imgUrl" alt="">
        <p>{{item.title}}</p>
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
   </div>
   </div>
</template>
<script>
export default {
  name: "HomeHot",
  props : ['list'],
  data() {
    return {
      swiperOption: {
        // 如果自行设计了插件，那么插件的一些配置相关参数，也应该出现在这个对象中，如下debugger
        debugger: true,
        //autoplay: 3000,
        slidesPerView: "auto" //设置slider容器能够同时显示的slides数量(carousel模式)。可以设置为数字（可为小数，小数不可loop），或者 'auto'则自动根据slides的宽度来设定数量。loop模式下如果设置为'auto'还需要设置另外一个参数loopedSlides。
        //   centeredSlides: true//<span style="color:rgb(68,68,68);font-family:'microsoft yahei';font-size:13px;">设定为true时，活动块会居中，而不是默认状态下的居左。</span>
      },
      imgList: [
        {
          imgSrc:
            "http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_150x150_8156d2ff.jpg",
          title: "上海迪斯尼乐园"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_150x150_8156d2ff.jpg",
          title: "上海迪斯尼乐园"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_150x150_8156d2ff.jpg",
          title: "上海迪斯尼乐园"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_150x150_8156d2ff.jpg",
          title: "上海迪斯尼乐园"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_150x150_8156d2ff.jpg",
          title: "上海迪斯尼乐园"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_150x150_8156d2ff.jpg",
          title: "上海迪斯尼乐园"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_150x150_8156d2ff.jpg",
          title: "上海迪斯尼乐园"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_150x150_8156d2ff.jpg",
          title: "上海迪斯尼乐园"
        }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
.hotp {
    background-color: #fff;
  .recommendtitle {
    margin-bottom: 0.2rem;
    margin-top: 0.2rem;
    .recommend-left {
      float: left;
      font-size: 0.36rem;
      margin-left: 0.2rem;
      margin-top: 0.2rem;
      font-weight: 700;
      img {
        width: 0.35rem;
      }
    }
    .recommend-right {
      float: right;
      margin-right: 0.2rem;
      margin-top: 0.2rem;
    }
  }
  .wrapper {
    .hotSwiper {
      width: 2rem;
      height: 2.4rem;
      margin-right: 0.1rem;
      margin-left: 0.1rem;
      img {
        width: 100%;
      }
      p {
        margin-top: 0.1rem;
        font-size: 0.12rem;
      }
      p:first-child {
        margin-left: 0.2rem;
      }
    }
  }
}
.clearfix:after {
  content: "";
  display: block;
  visibility: hidden;
  height: 0;
  clear: both;
}

.clearfix {
  zoom: 1;
}
</style>


