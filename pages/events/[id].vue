<template>
  <div>
    <h1>Event Details</h1>
    <p>Event ID: {{ $route.params.id }}</p>
  </div>
</template>

<script setup>
const nuxt = useNuxtApp()
console.log(nuxt)
</script>

<style scoped></style>
