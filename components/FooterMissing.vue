<template>
  <footer class="w-full py-6 bg-green-500">
    <div
      class="container flex flex-col items-center gap-2 px-4 text-center md:flex-row md:gap-4 md:px-6 lg:gap-0"
    >
      <div class="flex items-center space-x-2">
        <img
          src="https://images.unsplash.com/photo-1533738363-b7f9aef128ce?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Nnx8Y2F0fGVufDB8fDB8fHww"
          width="40"
          height="40"
          alt="Logo"
          class="rounded-full"
          style="aspect-ratio: 40 / 40; object-fit: cover"
        />
        <p class="text-xs font-semibold tracking-wide uppercase text-white">
          Missing Pets
        </p>
      </div>
      <nav class="flex flex-col gap-2 md:flex-row md:ml-auto md:gap-4 lg:gap-8">
        <a
          class="text-sm font-medium text-white transition-colors hover:underline dark:text-white dark:hover:underline"
          href="#"
        >
          Home
        </a>
        <a
          class="text-sm font-medium text-white transition-colors hover:underline dark:text-white dark:hover:underline"
          href="#"
        >
          Report a Missing Pet
        </a>
        <a
          class="text-sm font-medium text-white transition-colors hover:underline dark:text-white dark:hover:underline"
          href="#"
        >
          Found Pets
        </a>
        <a
          class="text-sm font-medium text-white transition-colors hover:underline dark:text-white dark:hover:underline"
          href="#"
        >
          Contact Us
        </a>
      </nav>
      <div class="flex items-center gap-4 md:gap-2 ml-auto">
        <a
          class="text-white dark:text-white hover:text-white dark:hover:text-white"
          href="#"
        >
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
            class="w-5 h-5"
          >
            <path
              d="M22 4s-.7 2.1-2 3.4c1.6 10-9.4 17.3-18 11.6 2.2.1 4.4-.6 6-2C3 15.5.5 9.6 3 5c2.2 2.6 5.6 4.1 9 4-.9-4.2 4-6.6 7-3.8 1.1 0 3-1.2 3-1.2z"
            ></path>
          </svg>
          <span class="sr-only">Twitter</span>
        </a>
        <a
          class="text-white dark:text-white hover:text-white dark:hover:text-white"
          href="#"
        >
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
            class="w-5 h-5"
          >
            <rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect>
            <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path>
            <line x1="17.5" x2="17.51" y1="6.5" y2="6.5"></line>
          </svg>
          <span class="sr-only">Instagram</span>
        </a>
        <a
          class="text-white dark:text-white hover:text-white dark:hover:text-white"
          href="#"
        >
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
            class="w-5 h-5"
          >
            <path
              d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"
            ></path>
          </svg>
          <span class="sr-only">Facebook</span>
        </a>
      </div>
    </div>
  </footer>
</template>
