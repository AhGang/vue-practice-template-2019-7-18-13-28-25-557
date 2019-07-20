<template>
  <div>
    <div v-for="i in inputNum" :key="i">
      <Counter  @calSum="calSum" />
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
     sum: 0
    }
  },
  methods:{
    calSum(data){
      this.sum += data;
      this.$emit("returnSum",this.sum)
    },
}
}
</script>

<style scoped>
</style>
