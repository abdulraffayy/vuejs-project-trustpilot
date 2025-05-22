<script setup lang="ts">
import logoimage from '../assets/logo.svg'
</script>

<template>
  <div class="w-full bg-black p-4 text-white">
    <div class="container mx-auto flex items-center justify-between">
      <div class="logo flex items-center space-x-2">
        <img :src="logoimage" alt="Logo" class="w-40 h-10"/>
      </div>

      <nav class="navbar">
        <ul class="flex items-center space-x-6 text-white">
          <li class="hover-underline cursor-pointer">Write a review</li>
          <li class="hover-underline cursor-pointer">Categories</li>
          <li class="hover-underline cursor-pointer">Blog</li>
          <li class="hover-underline cursor-pointer">Login</li>
          <li>
            <button
              class="bg-blue-100 rounded-md px-4 py-2 text-black cursor-pointer hover:bg-blue-900 hover:text-white"
            >
              For businesses
            </button>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<style scoped>
.hover-underline {
  position: relative;
}

.hover-underline::after {
  content: "";
  position: absolute;
  left: 0;
  right: 0;
  height: 2px;
  background-color: white;
  bottom: -23px; 
  opacity: 0;
  transition: opacity 0.3s ease;
}

.hover-underline:hover::after {
  opacity: 1;
}
</style>
