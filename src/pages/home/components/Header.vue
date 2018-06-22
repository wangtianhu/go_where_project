<template>
    <div class="header">
       <div class="header-left">
           <div class="iconfont icon-back"></div>
       </div>
       <div class="header-input">请输入目的地</div>
       <div class="header-right">城市</div>
    </div>

</template>
<script>
export default {
    nama:'HomeHeader'
}
</script>
  
   
<style lang="scss" scoped>
    $bgcolor: #00bcd4;
    .header{
        display: flex;
        height: 0.86rem;
        line-height: 0.86rem;
        background: $bgcolor;
        color: #fff;
        .header-left{
            width: 0.64rem;
            float: left;
        }
        .header-input{
            line-height:0.7rem;
            flex: 1;
            height: 0.64rem;
            margin-top: .12rem;
            margin-left: 0.2rem;
            background: #fff;
            border-radius: 0.1rem;
            color: #ccc;
        }
        .header-right{
            width: 1.28rem;
            float: right;
            text-align: center;
        }
    }
    
    

</style>

