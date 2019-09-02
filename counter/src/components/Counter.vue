<template>
  <div class="hello">

    <h2>Counter</h2>
    <p>
    <button @click="dec">-</button>
     <span>count{{count}}</span>
     <button @click="inc">+</button>
    </p>

  </div>
</template>

<script>
export default {
  
  //数据初始化
  data(){
        return {
          count:0
        }
  },  
 
  //事件处理函数
  methods:{
   
    //增加
    inc(){
      const count=this.count
      this.count=count+1
    },

    //减法
     dec(){
      const count=this.count
      this.count=count-1
    },
    
  }
}
</script>

<style scoped>

button{
  margin:0 20px; 
}
</style>