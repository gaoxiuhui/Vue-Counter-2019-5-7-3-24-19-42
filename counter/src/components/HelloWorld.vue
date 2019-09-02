<template>
  <div class="hello">    
    <ul>
    <li v-for="n in 30" :key="n">
     {{n}}<Counter></Counter>
    </li>
  </ul>  
  </div>
</template>

<script>
import Counter from './Counter.vue' 
export default {
  name: 'HelloWorld',
  components:{
    Counter
 }

}
</script>

<style scoped>


</style>
