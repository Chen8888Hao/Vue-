<template>
  <div>
<p>{{ reverseMessage}}</p>
<p>{{ reverseMessage}}</p>
<p>{{ reverseMessage}}</p>
<p>{{ reverseMessage}}</p>
<p>{{ reverseMessage}}</p>
<p>{{ getMessage()}}</p>
<p>{{ getMessage()}}</p>
<p>{{ getMessage()}}</p>
<p>{{ getMessage()}}</p>
<p>{{ getMessage()}}</p>
  </div>
</template>

<script>
export default {
data(){
    return{
    msg:"Hello,Vue"
    }
},
computed:{
    reverseMessage(){
        console.log("计算机属性执行了");
        return this.msg.split("").reverse().join("")
    }
},
methods:{
    getMessage(){
        console.log("函数属性执行了");
        return this.msg.split("").reverse().join("")
    }
}
}
</script>

<style>

</style>