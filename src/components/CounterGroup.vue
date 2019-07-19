<template>
  <div>
    <div v-for="i in inputNum" :key="i">
      <Counter/>
    </div>
  </div>

</template>

<script>
 import Counter from './Counter'
export default {
 name: 'CounterGroup',
 components:{
  Counter
 },
 props:['inputNum'],
 data(){
    return {
     
    }
  },
  methods:{
}
}
</script>

<style scoped>
</style>
