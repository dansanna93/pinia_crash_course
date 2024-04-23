<template>
  <div class="about">
    <h1>About</h1>
  </div>
  <button @click="storeCounter.increaseCount" class="counter-button">
    {{ storeCounter.count }}
  </button>
</template>

<script setup>
  import {useCounterStore} from '@/stores/counter'

  const storeCounter = useCounterStore()
</script>

<style>
  .counter-button {
    font-size: 50px;
  }
</style>