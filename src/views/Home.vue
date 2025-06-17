<script setup lang="ts">
import { useCounterStore } from "../stores/counter";
// biome-ignore lint/correctness/noUnusedVariables: <false positive>
const counter = useCounterStore();
</script>

<template>
  <div>
    <h1>Home</h1>
    <p>Count: {{ counter.count }}</p>
    <button @click="counter.increment">Increment</button>
  </div>
</template>

