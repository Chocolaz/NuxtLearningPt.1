<template>
  <div class="container mx-auto p-4">
    <header class="mb-6 text-center">
      <h1 class="text-5xl font-bold text-blue-600">
        Welcome to My Nuxt.js Project
      </h1>
      <p class="text-lg text-gray-700 mt-2">This is the home page.</p>
    </header>
    <main class="text-center">
      <div class="Main">
        <Alerts />
        <Profile />
      </div>
    </main>
  </div>
</template>

<script></script>

<style scoped>
.container {
  max-width: 800px;
}

button {
  transition: background-color 0.3s;
}
</style>
