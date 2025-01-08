<template>
  <div class="container py-3 mx-auto Main">
    <h1 class="text-teal-200">Main Page</h1>
  </div>
</template>

<script setup lang="ts">
const { $sayHello } = useNuxtApp()
$sayHello('Chocolate')
</script>
