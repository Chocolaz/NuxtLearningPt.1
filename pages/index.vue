<script setup>
import { ref } from 'vue'
import { useCounterStore } from '~/stores/myStore'
const { data } = await useFetch('/api/products')

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

const products = data.value.data.products
</script>

<template>
  <div class="container mx-auto p-4">
    <div id="main" class="mb-6">
      <h1 class="text-2xl font-bold mb-4">Counter: {{ counter }}</h1>
      <button
        @click="increment"
        class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600"
      >
        +
      </button>
      <button
        @click="decrement"
        class="px-4 py-2 bg-red-500 text-white rounded hover:bg-red-600 ml-2"
      >
        -
      </button>
    </div>
    <div id="products">
      <h2 class="text-xl font-semibold mb-4">Products</h2>
      <ul>
        <li
          v-for="product in products"
          :key="product.id"
          class="mb-2 p-4 bg-gray-100 rounded shadow"
        >
          <h3 class="text-lg font-bold text-red-500">{{ product.name }}</h3>
          <p class="text-gray-700">Price: ${{ product.price }}</p>
          <p class="text-gray-700">Description: {{ product.description }}</p>
          <p class="text-gray-700">Category: {{ product.category }}</p>
          <p class="text-gray-700">Stock: {{ product.stock }}</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.container {
  max-width: 800px;
}
</style>
