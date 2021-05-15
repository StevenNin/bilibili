<template>
  <div>
    <loginTop :topTitle="'注册账号'"></loginTop>
    <loginText 
    label="姓名" 
    style="margin:4.167vw 0"
    placeholder ="请输入姓名"
    rule="^.{6,16}$"
    >
    </loginText>
    <loginText  label="账号"  placeholder ="请输入账号" rule="^.{6,16}$"></loginText>
    <loginText  label="密码"  placeholder ="请输入密码" type="password"  rule="^.{6,16}$"></loginText>

    <div class="btnBox">
      <loginBtn  name="注册"></loginBtn>
    </div>
  </div>
</template>

<script>
import loginTop from "@/components/common/loginTop.vue"
import loginText from "@/components/common/loginText.vue"
import loginBtn from "@/components/common/loginBtn.vue"

export default {
    name:"register",
    components:{loginTop,loginText,loginBtn},
}
</script>

<style>

</style>