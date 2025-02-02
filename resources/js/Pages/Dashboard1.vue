<template>
    <div class="container mx-auto px-4">
      <!-- Navbar -->
      <nav class="flex justify-between items-center py-4">
        <div class="text-2xl font-bold">Logo</div>
        <ul class="flex space-x-4">
          <li><a href="#" class="hover:underline">Home</a></li>
          <li><a href="#" class="hover:underline">Explore</a></li>
          <li><a href="#" class="hover:underline">About</a></li>
          <li><a href="#" class="hover:underline">Login/Signup</a></li>
        </ul>
      </nav>
  
      <!-- Hero Section -->
      <section class="text-center py-16">
        <h1 class="text-4xl font-bold mb-4">🚀 Share Your Side Projects & Get Inspired!</h1>
        <div class="space-x-4">
          <button class="bg-blue-500 text-white px-4 py-2 rounded-lg">Post a Project</button>
          <button class="bg-gray-200 px-4 py-2 rounded-lg">Explore Projects</button>
        </div>
      </section>
  
      <!-- Projects Section -->
      <section class="py-8">
        <h2 class="text-2xl font-bold">🔥 Trending Projects | 🆕 Latest Projects</h2>
        <div class="grid grid-cols-3 gap-4 mt-4">
          <div v-for="i in 6" :key="i" class="border rounded-lg p-4">
            <h3 class="font-semibold">Project Title {{ i }}</h3>
            <p class="text-gray-600">Short description of the project...</p>
          </div>
        </div>
      </section>
  
      <!-- Featured Project -->
      <section class="py-8">
        <h2 class="text-2xl font-bold">⭐ Featured Project of the Week</h2>
        <div class="border rounded-lg p-6 mt-4">
          <h3 class="font-semibold text-xl">Amazing Project Title</h3>
          <p class="text-gray-600">Detailed description of the featured project...</p>
        </div>
      </section>
  
      <!-- Leaderboard & Top Contributors -->
      <section class="py-8">
        <h2 class="text-2xl font-bold">🏆 Leaderboard | 🎖️ Top Contributors</h2>
        <div class="grid grid-cols-3 gap-4 mt-4">
          <div v-for="i in 3" :key="i" class="flex items-center space-x-4">
            <div class="w-10 h-10 bg-gray-300 rounded-full"></div>
            <div>
              <h4 class="font-semibold">User Name {{ i }}</h4>
              <p class="text-gray-600">Score: {{ i * 100 }}</p>
            </div>
          </div>
        </div>
      </section>
  
      <!-- Call to Action -->
      <section class="text-center py-16 bg-gray-100">
        <h2 class="text-2xl font-bold">📢 Join the Community & Share Your Ideas!</h2>
        <button class="bg-green-500 text-white px-4 py-2 rounded-lg mt-4">Get Started for Free</button>
      </section>
  
      <!-- Footer -->
      <footer class="py-4 text-center">
        <div class="space-x-4">
          <a href="#" class="hover:underline">About</a>
          <a href="#" class="hover:underline">Contact</a>
          <a href="#" class="hover:underline">Privacy Policy</a>
        </div>
        <div class="mt-4">
          <span class="mx-2">🔗</span>
          <span class="mx-2">🔗</span>
          <span class="mx-2">🔗</span>
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
  .container {
    max-width: 1200px;
  }
  </style>
  
  