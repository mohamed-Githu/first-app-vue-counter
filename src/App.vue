<script setup>
import { ref } from 'vue';

const count = ref(0);
</script>

<template>
  <div class="container">
    <h4>Current Count</h4>
    <h1>{{ count }}</h1>
    <div class="buttons-container">
      <button @click="count--">-</button>
      <button @click="count++">+</button>
    </div>
  </div>
</template>

<style scoped>
button {
  margin: 0 5px;
  cursor: pointer;
  font-size: 1.5rem;
  border-radius: 999px;
  height: 40px;
  width: 40px;
  text-align: center;
  outline: none;
  border: none;
}

.buttons-container {
  margin-top: 20px;
}

h4 {
  margin-bottom: 10px;
  font-size: 2rem;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}
</style>