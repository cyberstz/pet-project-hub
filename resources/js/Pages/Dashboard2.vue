<template>
  <div class="bg-gray-100 min-h-screen">
      <!-- Navbar -->
      <nav class="flex items-center justify-between p-4 bg-white shadow-md">
      <div class="flex items-center space-x-4">
          <img src="/logo.png" alt="Logo" class="h-8">
          <a href="#" class="text-lg font-semibold">Home</a>
          <a href="#" class="text-lg">Explore</a>
          <a href="#" class="text-lg">About</a>
      </div>
      <div>
          <button class="px-4 py-2 bg-blue-500 text-white rounded-lg">Login/Signup</button>
      </div>
      </nav>

      <!-- Hero Section -->
      <section class="text-center py-16 bg-blue-100">
      <h1 class="text-4xl font-bold mb-4">🚀 Share Your Side Projects & Get Inspired!</h1>
      <div class="space-x-4">
          <button class="px-6 py-2 bg-green-500 text-white rounded-lg">Post a Project</button>
          <button class="px-6 py-2 bg-blue-500 text-white rounded-lg">Explore Projects</button>
      </div>
      </section>

      <!-- Trending & Latest Projects -->
      <section class="p-8">
      <div class="flex justify-between mb-4">
          <h2 class="text-2xl font-bold">🔥 Trending Projects</h2>
          <h2 class="text-2xl font-bold">🆕 Latest Projects</h2>
      </div>
      <div class="grid grid-cols-3 gap-4">
          <div class="bg-white p-4 rounded-lg shadow-md" v-for="n in 6" :key="n">
          <h3 class="font-semibold">Project Title {{n}}</h3>
          <p class="text-gray-500">Short project description...</p>
          <div class="flex justify-between items-center mt-2">
              <span>🔥 120</span>
              <span>💬 45</span>
          </div>
          </div>
      </div>
      </section>

      <!-- Featured Project of the Week -->
      <section class="p-8 bg-yellow-100">
      <h2 class="text-3xl font-bold mb-4">⭐ Featured Project of the Week</h2>
      <div class="bg-white p-6 rounded-lg shadow-lg">
          <h3 class="text-2xl font-semibold">Amazing Project Title</h3>
          <p class="text-gray-600">Detailed description of the featured project...</p>
      </div>
      </section>

      <!-- Leaderboard & Top Contributors -->
      <section class="p-8">
      <div class="flex justify-between">
          <div>
          <h2 class="text-2xl font-bold">🏆 Leaderboard</h2>
          <div class="mt-4" v-for="n in 3" :key="n">
              <div class="flex items-center space-x-2">
              <img src="/avatar.png" alt="Avatar" class="h-8 w-8 rounded-full">
              <span class="font-semibold">User {{n}}</span>
              <span class="text-gray-500">Score: {{n * 100}}</span>
              </div>
          </div>
          </div>

          <div>
          <h2 class="text-2xl font-bold">🎖️ Top Contributors</h2>
          <div class="mt-4" v-for="n in 3" :key="n">
              <div class="flex items-center space-x-2">
              <img src="/avatar.png" alt="Avatar" class="h-8 w-8 rounded-full">
              <span class="font-semibold">Contributor {{n}}</span>
              <span class="text-gray-500">Projects: {{n * 5}}</span>
              </div>
          </div>
          </div>
      </div>
      </section>

      <!-- Call to Action -->
      <section class="text-center py-16 bg-green-100">
      <h2 class="text-3xl font-bold mb-4">📢 Join the Community & Share Your Ideas!</h2>
      <button class="px-6 py-2 bg-blue-500 text-white rounded-lg">Get Started for Free</button>
      </section>

      <!-- Footer -->
      <footer class="p-4 bg-gray-200 text-center">
      <p>&copy; 2025 Pet Project Hub. All rights reserved.</p>
      <div class="flex justify-center space-x-4 mt-2">
          <a href="#" class="text-gray-600">About</a>
          <a href="#" class="text-gray-600">Contact</a>
          <a href="#" class="text-gray-600">Privacy Policy</a>
      </div>
      </footer>
  </div>
  </template>

  <script>
  export default {
  name: 'HomePage',
  };
  </script>

  <style scoped>
  body {
  font-family: 'Arial', sans-serif;
  }
  </style>