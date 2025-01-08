<template>
  <nav class="bg-blue-600">
    <h1 class="text-white text-2xl font-bold">My Nuxt Project</h1>
    <ul class="flex space-x-4">
      <li>
        <NuxtLink to="/" class="text-white hover:underline">Home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/events" class="text-white hover:underline"
          >Events</NuxtLink
        >
      </li>
    </ul>
  </nav>
</template>
