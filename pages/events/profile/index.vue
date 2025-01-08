<template>
  <div class="container mx-auto p-4">
    <header class="mb-6 text-center">
      <h1 class="text-4xl font-bold text-blue-600">My Profile</h1>
      <p class="text-lg text-gray-700 mt-2">Welcome to your profile page!</p>
    </header>
    <main class="text-center">
      <div class="profile-card p-6 bg-white shadow rounded">
        <img
          class="w-24 h-24 rounded-full mx-auto"
          src="https://i.pinimg.com/736x/4e/12/14/4e121415eaf935aba51d543058de94d7.jpg"
          alt="Profile Picture"
        />
        <h2 class="text-2xl font-semibold mt-4">Gomen Armanai</h2>
        <p class="text-gray-600">gomen@example.com</p>
      </div>
    </main>
  </div>
</template>

<script></script>

<style scoped>
.container {
  max-width: 600px;
}
.profile-card {
  max-width: 400px;
  margin: 0 auto;
}
</style>
