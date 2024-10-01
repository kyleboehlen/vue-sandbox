<template>
  <button @click="clickMe">
    Click me maybe?
  </button>
</template>

<script setup>
import {useCounterStore} from "@/stores/counter.js";
const counter = useCounterStore()
const clickMe = () => {
  counter.increment()
}
</script>

<style scoped>
button {
  color: var(--vt-c-white);
  font-size: 1.25em;
  background-color: var(--vt-c-divider-dark-2);
  width: 10vw;
  height: 5vh;
  border-radius: 5px;
  border-color: var(--vt-c-indigo)
}

button:hover {
  cursor: pointer;
}
</style>