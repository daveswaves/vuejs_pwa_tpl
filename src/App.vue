<!-- App.vue -->
<script setup>
// 'vue-router' import not required because Vue 3 automatically registers certain built-in components globally
// when using Single File Components (SFCs) and <script setup>. This includes RouterLink and RouterView
// import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="min-h-screen bg-white text-black dark:bg-gray-900 dark:text-white">
    <nav class="p-4 bg-gray-200 dark:bg-gray-800 flex gap-4">
      <RouterLink to="/" class="text-xl text-blue-500">Home</RouterLink>
      <RouterLink to="/about" class="text-xl text-green-500">About</RouterLink>
    </nav>
    
    <!-- Dynamically renders HomeView component contents or AboutView component contents here -->
    <RouterView />
  </div>
</template>
