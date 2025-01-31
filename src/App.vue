<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav class="flex justify-between items-center px-[50px] py-[15px] bg-gray-800 text-white">
    <div>
      <RouterLink to="/" class="text-2xl font-semibold">FKN.</RouterLink>
    </div>
    <div class="flex space-x-6">
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/projects">Projects</RouterLink>
      <RouterLink to="/blog">Blog</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
      <button class="cursor-pointer flex items-center justify-center">
        <span style="font-size: 20px;" class="material-symbols-outlined">search</span>
      </button>
    </div>
  </nav>

  <RouterView />
  <div class="text-6xl text-emerald-500 font-mono">
    You're Awesome! 🚀
  </div>
  <div>
    <span class="material-symbols-outlined text-4xl text-blue-500">
      home
    </span>
    <p class="mt-2">Ini icon rumah!</p>
  </div>
</template>