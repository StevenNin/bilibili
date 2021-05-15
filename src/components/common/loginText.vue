<template>
  
  <div class="input">
      <van-field v-model="text" 
      :label="label" :type="type" :placeholder="placeholder" :rule="rule" />
  </div>
</template>

<script>
export default {
    name:"loginText",
    props:["label", "type","placeholder","rule" ],
    data(){
        return{
            text:'',
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
    .input{
        // height: 50px;
        // border: 1px solid red;
        display: flex;
        background-color: @backcolor;
        border: 1px solid #000000;
        padding: 10px 5px;
    }
</style>