<template>
  <div class="container py-3 mx-auto Main">
    <ContentDoc />
  </div>
</template>

<script setup lang="ts">
definePageMeta({ middleware: 'auth' })
</script>
