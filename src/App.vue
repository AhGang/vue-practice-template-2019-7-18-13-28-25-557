<template>
  <div>
    <input id="mInput" v-model.number="inputNum">
    <div>
      <CounterGrop :inputNum = "inputNum"></CounterGrop>
    </div>
    
  </div>
</template>

<script>
import CounterGrop from './components/CounterGroup'
export default {
  components:{
    CounterGrop
  },
  name: 'app',
  data(){
    return {
      inputNum : 0,
    }
  },
  methods:{
  }
}


</script>

<style>

</style>
