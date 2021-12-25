<template>
  <div>
      <span>姓名：</span>
      <input type="text" v-model="full">
  </div>
</template>

<script>
export default {
data(){
    return{

    }
},
computed:{
    full:{
    set(val){
        console.log(val);
    }   ,
    gte(){
        return "无名氏"
    } 
    }
}
}
</script>

<style>

</style>