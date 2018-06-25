<template>
    <div class="homeweekend">
        <div class="week-title">
            周末推荐
        </div>
        <div class="week-reco">
            <ul>
                <li>
                    <div class="weekImg">
                        <img src="http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg" alt="">
                    </div>
                    <div class="weekContent">
                        <p>上海必游TOP10</p>
                        <p>中西完美合璧，展现现代上海风貌</p>
                    </div>
                </li>
                <li>
                    <div class="weekImg">
                        <img src="http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg" alt="">
                    </div>
                    <div class="weekContent">
                        <p>上海必游TOP10</p>
                        <p>中西完美合璧，展现现代上海风貌</p>
                    </div>
                </li>
                <li>
                    <div class="weekImg">
                        <img src="http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg" alt="">
                    </div>
                    <div class="weekContent">
                        <p>上海必游TOP10</p>
                        <p>中西完美合璧，展现现代上海风貌</p>
                    </div>
                </li>
                <li>
                    <div class="weekImg">
                        <img src="http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg" alt="">
                    </div>
                    <div class="weekContent">
                        <p>上海必游TOP10</p>
                        <p>中西完美合璧，展现现代上海风貌</p>
                    </div>
                </li>
                <li>
                    <div class="weekImg">
                        <img src="http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg" alt="">
                    </div>
                    <div class="weekContent">
                        <p>上海必游TOP10</p>
                        <p>中西完美合璧，展现现代上海风貌</p>
                    </div>
                </li>
                <li>
                    <div class="weekImg">
                        <img src="http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg" alt="">
                    </div>
                    <div class="weekContent">
                        <p>上海必游TOP10</p>
                        <p>中西完美合璧，展现现代上海风貌</p>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
  name: "HomeWeekend"
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
