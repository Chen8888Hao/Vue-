<template>
  <div>
      <p>原来的样子:{{msg}}</p>
      <p>使用翻转过滤器：{{msg | reverse("|") }}</p>
      <p :title="msg | toUp | reverse('|')">鼠标长停</p>
  </div>
</template>

<script>
export default {
data(){
    return{
        msg: "Hello,vue"
    }
},
 filters:{
    toUp (val){
           return val.toUpperCase();
    }
 }
}
</script>

<style>

</style>