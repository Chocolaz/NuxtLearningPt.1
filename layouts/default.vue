<template>
  <div class="min-h-screen flex flex-col bg-gray-100">
    <header class="bg-blue-600 text-white p-4">
      <div class="container mx-auto flex justify-between items-center">
        <h1 class="text-2xl font-bold">My Nuxt Project</h1>
        <nav>
          <ul class="flex space-x-4">
            <li>
              <NuxtLink to="/" class="hover:underline">Home</NuxtLink>
            </li>
          </ul>
        </nav>
      </div>
    </header>
    <main class="flex-grow container mx-auto p-4">
      <slot />
    </main>
    <footer class="bg-gray-800 text-white p-4">
      <div class="container mx-auto text-center">
        <p>&copy; My First Nuxt Project.</p>
      </div>
    </footer>
  </div>
</template>
