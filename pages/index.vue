<script setup>
import { ref } from 'vue'
import { useCounterStore } from '~/stores/myStore'

const store = useCounterStore()
const counter = ref(store.count)

const increment = () => {
  store.increment()
  counter.value = store.count
}

const decrement = () => {
  store.decrement()
  counter.value = store.count
}

console.log(store)
</script>

<template>
  <div>
    <div id="main">
      Counter: {{ counter }}
      <button @click="increment">+</button>
      <button @click="decrement">-</button>
    </div>
    <Counter id="counter" />
  </div>
</template>
