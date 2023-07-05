<template>
  <main>
    <div>
      <h4>The current counter value is ... </h4>
      <h1>{{ count }}</h1>
      <button @click="increment()">+</button>
      <button @click="decrement()">-</button>
    </div>
  </main>
</template>

<!-- <script setup>
import { ref } from "vue"
const count = ref(0);
const increment = () => {
  count.value = count.value + 1;
}
const decrement = () => {
  count.value = count.value - 1;
}
</script> -->

<script>
export default({
  data() {
    return {
      count: 0
    }
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    }
  }
});
</script>

<style scoped>
main {
  background-color: aliceblue;
  width: 80vw;
  height: 80vh;
  padding: 10px;
}
</style>
