<template>
  <div class="bg-green-700 py-2 text-white">
    <div class="container mx-auto flex justify-between items-center py-4">
      <div class="px-6 flex justify-center items-center">
        <UIcon name="i-material-symbols-pets" dynamic class="h-8 w-8 mr-4" />
        <router-link to="/" class="text-lg font-bold">My App</router-link>
      </div>
      <div class="flex space-x-4 px-8">
        <router-link to="/about" class="hover:text-gray-300">About</router-link>
        <router-link to="/contact" class="hover:text-gray-300"
          >Contact</router-link
        >
      </div>
    </div>
  </div>
</template>
