<template>
  <div>
    <Counter @add="add1"></Counter>
  </div>
</template>

<script>
import Counter from './components/CounterBody.vue'

export default {
  data() {
    return {
      count1: 0,
    }
  },
  components: {
    Counter
  },
  methods: {
    add1(count) {
      this.count1 = count;
    }
  }
}
</script>