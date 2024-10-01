<script setup>
import {useCounterStore} from "@/stores/counter.js";
const counter = useCounterStore()

const resetCounter = () => {
  counter.zero()
}
</script>

<template>
  <p>This uses a Pinia store: <span class="indigo">{{ counter.count }}</span></p>
  <p v-if="counter.count > 0" class="reset" @click="resetCounter">Reset</p>
</template>

<style scoped>
p {
  margin: 30px;
}
span.indigo {
  color: var(--vt-c-indigo);
}
p.reset {
  color: var(--vt-c-white);
  text-decoration: underline;
}
p.reset:hover {
  cursor: pointer;
  color: var(--vt-c-indigo);
}
</style>