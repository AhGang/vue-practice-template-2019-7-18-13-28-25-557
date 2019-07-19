<template>
  <div id="app">
    <button @click="increase()">+</button>
     <input id="num1" v-model="calNumber">
    <button @click="decrease()">-</button>
  </div>
</template>

<script>
export default {
 name: 'HelloWorld',
 data(){
    return {
      calNumber: 0
    }
  },
  methods:{
  increase(){
      this.calNumber++;
     },
  decrease(){
      if(this.calNumber>0){
        this.calNumber--;
      }
  }
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
