<template>
    <div class="homeIcons">
        <div class="icons" v-for="(item,index) in list" :key="index">
            <img :src="item.imgUrl" alt="">
            <p>{{item.desc}}</p>
        </div>
    </div>
</template>
<script>
export default {
  name: "HomeIcons",
  props:{
    list:Array
  },
  data() {
    return {
      iconsList: [
        {
          imgSrc:
            "http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png",
          title: "景点门票"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png",
          title: "一日游"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png",
          title: "必游榜单"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/piao/fusion/1803/76/eb88861d78fb9902.png",
          title: "夏日玩水"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/piao/fusion/1803/6a/45f595250c73d102.png",
          title: "普陀山"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png",
          title: "每日精选"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/piao/fusion/1803/b1/528a9e80403b8c02.png",
          title: "动物园"
        },
        {
          imgSrc:
            "http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png",
          title: "一日游"
        }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
.homeIcons {
  width: 100%;
  overflow: hidden;
  padding-bottom: 50%;
  height: 0;
  background-color: #fff;
  .icons {
    float: left;
    width: 25%;
    padding-bottom: 25%;
    color: red;
    height: 0;
    box-sizing: border-box;
    img {
      width: 1.1rem;
      height: 1.1rem;
      display: inline-block;
      margin-top: 0.2rem;
    }
    p{
        color: black;
    }
  }
}
</style>
