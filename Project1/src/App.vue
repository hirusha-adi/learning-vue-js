<script setup>

import { ref } from "vue";
const count = ref(0);

const addCount = () => {
  console.log("Add count");
  count.value += 1;
}

const subCount = () => {
  console.log("Sub count");
  count.value -= 1;
}

</script>

<template>
  <div>
    <h4>The current count is ...</h4>
    <h1>{{ count }}</h1>
    <button @click="subCount()">-</button>
    <button @click="addCount()">+</button>
  </div>
</template>

<style scoped>
button {
  width: 10vh;
  margin: 1vh;
}
</style>