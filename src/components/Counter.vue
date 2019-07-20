<template>
<div>
    <button @click="calSum(1)">+</button>
     <input id="num1" v-model="calNumber">
    <button @click="calSum(-1)">-</button>
  </div>
</template>

<script>
export default {
 name: 'Counter',
 data(){
    return {
     calNumber: 0,
    }
  },
  methods:{
  calSum(data){
      this.calNumber += data;
      data>0? this.$emit("calSum",1):this.$emit("calSum",-1)
     }
}
}
</script>

<style scoped>
</style>
