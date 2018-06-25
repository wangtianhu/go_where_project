<template>
    <div class="homeweekend">
        <div class="week-title">
            周末推荐
        </div>
        <div class="week-reco">
            <ul>
                <li v-for="(item,index) in list" :key="index">
                    <div class="weekImg">
                        <img :src="item.imgUrl" alt="">
                    </div>
                    <div class="weekContent">
                        <p>{{item.title}}</p>
                        <p>{{item.desc}}</p>
                    </div>
                </li>

            </ul>
        </div>
    </div>
</template>
<script>
export default {
  name: "HomeWeekend",
  props : ['list']
};
</script>
<style lang="scss" scoped>
.homeweekend {
  .week-title {
    font-size: 0.36rem;
    margin-top: 0.2rem;
    margin-bottom: 0.2rem;
    margin-left: -5rem;
  }
  .week-reco ul li{
      background-color: #fff;
      .weekImg{
          width: 100%;
          height: 2.8rem;
          img{
              height: 2.8rem;
          }
      }
      .weekContent{
          padding: 0.14rem 0.2rem 0.2rem 0.2rem;
          box-sizing: border-box;
          p:first-child{
              margin-left: -5rem;
             line-height: 0.5rem;
          }
           p:last-child{
               margin-left: -3.4rem;
              font-size: 0.2rem;
         }
           }
      }
  }

</style>
