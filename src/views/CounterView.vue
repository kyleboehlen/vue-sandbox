<template xmlns="http://www.w3.org/1999/html">
  <div class="counter">
    <CounterButton></CounterButton>
    <CounterDisplay></CounterDisplay>
  </div>
</template>

<script setup>
import CounterButton from "@/components/CounterButton.vue";
import CounterDisplay from "@/components/CounterDisplay.vue";

</script>

<style>
@media (min-width: 1024px) {
  .counter {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>