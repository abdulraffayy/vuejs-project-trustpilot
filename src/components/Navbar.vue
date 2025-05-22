<script setup lang="ts">
import logoimage from '../assets/logo.svg'
</script>

<template>
  <div class="w-full bg-red-300 p-4">
    <div class="container mx-auto flex items-center justify-between">
      <div class="logo flex items-center space-x-2">
        <img :src="logoimage" alt="Logo" class="w-40 h-10"/>
      </div>

      <nav class="navbar">
        <ul class="flex space-x-6 text-white">
          <li class="cursor-pointer hover:">Write a review</li>
          <li class="cursor-pointer hover:underline">Categories</li>
          <li class="cursor-pointer hover:underline">Blog</li>
          <li class="cursor-pointer hover:underline">Login</li>
        </ul>
      </nav>

      <div class="button">
        <button class="bg-white text-red-500 px-4 py-2 rounded hover:bg-gray-100">
          For businesses
        </button>
      </div>
    </div>
  </div>
</template>
