<template>
  <div
    class="rounded-lg border bg-card text-card-foreground shadow-sm w-full max-w-sm"
    data-v0-t="card"
  >
    <div class="p-0">
      <img
        :src="props.image"
        width="400"
        height="250"
        alt="Pet"
        class="aspect-video overflow-hidden"
      />
    </div>
    <div class="p-4">
      <div class="flex items-center space-x-4">
        <h3 class="text-lg font-bold">{{ props.title }}</h3>
        <div
          class="inline-flex items-center rounded-full whitespace-nowrap border px-2.5 py-0.5 w-fit text-xs font-semibold transition-colors focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 text-foreground"
        >
          {{ props.type }}
        </div>
      </div>
      <p class="text-sm text-gray-500 dark:text-gray-400">
        {{ props.description }}
      </p>
    </div>
    <div
      class="bg-gray-100 dark:bg-gray-800 p-4 flex items-center justify-between"
    >
      <div class="flex items-center space-x-2">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="h-4 w-4 opacity-70"
        >
          <polygon points="3 6 9 3 15 6 21 3 21 18 15 21 9 18 3 21"></polygon>
          <line x1="9" x2="9" y1="3" y2="18"></line>
          <line x1="15" x2="15" y1="6" y2="21"></line>
        </svg>
        <span class="text-xs font-medium">{{ props.location }}</span>
      </div>
      <button
        class="inline-flex items-center text-white justify-center whitespace-nowrap text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-9 rounded-md px-3"
      >
        Contact
      </button>
    </div>
  </div>
</template>

<script setup>
const props = defineProps([
  "title",
  "description",
  "image",
  "location",
  "type",
]);
</script>
