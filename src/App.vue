<template>
  <div>
    <input v-model.number="inputNum">
    <div>
      <CounterGrop :inputNum = "inputNum"  @returnSum="getSum"></CounterGrop>
    </div>
    <div>
      <CounterSum :sum="sum"/>
    </div>
  </div>
</template>

<script>
import CounterGrop from './components/CounterGroup'
import CounterSum from './components/CounterSum'
export default {
  components:{
    CounterGrop,
    CounterSum
  },
  name: 'app',
  data(){
    return {
      inputNum : 0,
      sum: 0
    }
  },
  computed:{

  },
  methods:{
    getSum(data){
      this.sum = data;
    }
  }
}
</script>
