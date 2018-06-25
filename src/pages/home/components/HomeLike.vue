<template>
    <div class="hotlike">
        <ul>
            <li v-for="item in list">
                <div class="hotlike-left">
                    <img :src="item.imgUrl" alt="">
                </div>
                <div class="hotlick-right">
                    <div class="hotlike-title">
                        {{item.title}}
                    </div>
                    <div class="hotPj">
                        5115条评论
                    </div>
                    <div class="hotsell">
                        <div class="sellLeft">
                            <span>￥</span><span>236</span>起
                        </div>
                        <div class="sellRight">
                            浦东新区
                        </div>
                    </div>
                </div>
            </li>

            
          
            
        </ul>
    </div>
</template>
<script>
export default {
  name: "HomeLike",
  props:['list']
};
</script>
<style lang="scss" scoped>
.hotlike li {
  padding: 0.2rem;
  display: flex;
  justify-content: space-between;
  background: #fff;
  .hotlike-left {
    width: 2rem;
    img {
      width: 100%;
    }
  }
  .hotlick-right {
    width: 5rem;
    padding: 0.2rem 0.2rem 0.1rem 0.1rem;
    box-sizing: border-box;
    .hotlike-title{
        margin-left: -2rem;
        font-size: 0.32rem;
    }
    .hotPj{
        margin-top: 0.5rem;
        margin-left: -3.5rem;
        font-size: 0.2rem;
    }
    .hotsell{
        display: flex;
        margin-top: 0.3rem;
        justify-content: space-between;
        .sellLeft{
            span{
                color: red;
            }
            span:last-child{
                font-size: 0.4rem;
            }

        }
    }
  }
}
</style>
