<template>
  <main class="main max-w-400">

    <h1>Contador</h1>
    <br>
    <button @click="decrement">➖️</button>
    <span>{{ counter }}</span>
    <button @click="increment">➕️</button>
    
  </main>
</template>

<script setup lang="ts">

import { ref } from 'vue'

const counter = ref<number>(0)
const decrement = () : boolean | number => (counter.value > 0) && counter.value--
const increment = () : number => counter.value++

</script>

<style scoped>

h1 {
  text-decoration: underline;
}

span {
  margin: 0 1rem;
  font-size: 1.8rem;
  font-weight: bold;
}

</style>