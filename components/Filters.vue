<template>
  <section class="px-4 md:px-6 py-6 md:py-12 grid gap-6 md:gap-12 items-start">
    <div class="container grid gap-6 md:gap-12 items-start">
      <div
        class="flex flex-col md:flex-row items-start md:items-center gap-4 md:gap-8"
      >
        <div class="flex flex-col md:flex-row gap-4 md:gap-8 min-w-0">
          <div class="flex items-center gap-2">
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
              class="w-4 h-4 text-gray-500 dark:text-gray-400"
            >
              <polygon
                points="3 6 9 3 15 6 21 3 21 18 15 21 9 18 3 21"
              ></polygon>
              <line x1="9" x2="9" y1="3" y2="18"></line>
              <line x1="15" x2="15" y1="6" y2="21"></line>
            </svg>
            <input
              class="flex h-10 rounded-md border border-input bg-background px-3 py-2 ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 w-full max-w-xs text-sm"
              placeholder="Enter your location"
              type="text"
            />
          </div>
          <div class="flex items-center gap-2">
            <button
              class="flex items-center bg-white rounded-full border-2 py-2 px-4 mr-6"
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
                class="w-4 h-4 text-gray-500 dark:text-gray-400"
              >
                <path
                  d="M10 5.172C10 3.782 8.423 2.679 6.5 3c-2.823.47-4.113 6.006-4 7 .08.703 1.725 1.722 3.656 1 1.261-.472 1.96-1.45 2.344-2.5"
                ></path>
                <path
                  d="M14.267 5.172c0-1.39 1.577-2.493 3.5-2.172 2.823.47 4.113 6.006 4 7-.08.703-1.725 1.722-3.656 1-1.261-.472-1.855-1.45-2.239-2.5"
                ></path>
                <path d="M8 14v.5"></path>
                <path d="M16 14v.5"></path>
                <path d="M11.25 16.25h1.5L12 17l-.75-.75Z"></path>
                <path
                  d="M4.42 11.247A13.152 13.152 0 0 0 4 14.556C4 18.728 7.582 21 12 21s8-2.272 8-6.444c0-1.061-.162-2.2-.493-3.309m-9.243-6.082A8.801 8.801 0 0 1 12 5c.78 0 1.5.108 2.161.306"
                ></path>
              </svg>
              <option value="dog">Dogs</option>
            </button>
            <button
              class="flex items-center bg-white rounded-full border-2 py-2 px-4"
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
                class="w-4 h-4 text-gray-500 dark:text-gray-400"
              >
                <path
                  d="M12 5c.67 0 1.35.09 2 .26 1.78-2 5.03-2.84 6.42-2.26 1.4.58-.42 7-.42 7 .57 1.07 1 2.24 1 3.44C21 17.9 16.97 21 12 21s-9-3-9-7.56c0-1.25.5-2.4 1-3.44 0 0-1.89-6.42-.5-7 1.39-.58 4.72.23 6.5 2.23A9.04 9.04 0 0 1 12 5Z"
                ></path>
                <path d="M8 14v.5"></path>
                <path d="M16 14v.5"></path>
                <path d="M11.25 16.25h1.5L12 17l-.75-.75Z"></path>
              </svg>
              <option value="cat">Cats</option>
            </button>
          </div>
          <div class="flex items-center gap-2">
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
              class="w-4 h-4 text-gray-500 dark:text-gray-400"
            >
              <path
                d="M10 5.172C10 3.782 8.423 2.679 6.5 3c-2.823.47-4.113 6.006-4 7 .08.703 1.725 1.722 3.656 1 1.261-.472 1.96-1.45 2.344-2.5"
              ></path>
              <path
                d="M14.267 5.172c0-1.39 1.577-2.493 3.5-2.172 2.823.47 4.113 6.006 4 7-.08.703-1.725 1.722-3.656 1-1.261-.472-1.855-1.45-2.239-2.5"
              ></path>
              <path d="M8 14v.5"></path>
              <path d="M16 14v.5"></path>
              <path d="M11.25 16.25h1.5L12 17l-.75-.75Z"></path>
              <path
                d="M4.42 11.247A13.152 13.152 0 0 0 4 14.556C4 18.728 7.582 21 12 21s8-2.272 8-6.444c0-1.061-.162-2.2-.493-3.309m-9.243-6.082A8.801 8.801 0 0 1 12 5c.78 0 1.5.108 2.161.306"
              ></path>
            </svg>
            <input
              class="flex h-10 rounded-md border border-input bg-background px-3 py-2 ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 w-full max-w-xs text-sm"
              placeholder="Enter race"
              type="text"
            />
          </div>
        </div>
        <div class="flex items-center gap-4">
          <input
            class="flex h-10 rounded-md border border-input bg-background px-3 py-2 text-sm ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 max-w-sm w-full"
            placeholder="Search for pets"
            type="text"
          />
          <button
            class="inline-flex bg-green-600 text-white items-center justify-center whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 border border-input bg-background hover:bg-accent hover:text-accent-foreground h-10 px-4 py-2 shrink-0"
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
              class="w-4 h-4 mr-2"
            >
              <circle cx="11" cy="11" r="8"></circle>
              <path d="m21 21-4.3-4.3"></path>
            </svg>
            Search
          </button>
        </div>
      </div>
    </div>
  </section>
</template>
