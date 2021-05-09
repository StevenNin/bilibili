<template>
  
  <div class="navTop">
      <div></div>
      <div>{{topTitle}}</div>
      <div></div>
  </div>
</template>

<script>
export default {
    name:"loginTop",
    props:{
        topTitle:{
            type:String,
        },
    },
    data(){
        return{

        }
    },
}
</script>

<style lang="less" scoped>
@import "../../assets/base.less";
    .navTop{
        height: 50px;
        // border: 1px solid red;
        display: flex;
        background-color: @themeColor;
        div{
            color: @backcolor;
            display: flex;
            flex: 1;
            justify-content: center;
            align-items: center;    
            font-size: 4vw; 
        }
    }
</style>