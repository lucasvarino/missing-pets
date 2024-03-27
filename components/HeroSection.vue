<template>
  <section class="w-full py-12 md:py-24 bg-white text-black">
    <div class="container flex flex-col items-center gap-4 px-4 md:px-10">
      <div class="grid items-center gap-4 md:grid-cols-2">
        <div class="space-y-2">
          <h1
            class="text-3xl font-bold tracking-tighter sm:text-4xl md:text-5xl xl:text-6xl/none"
          >
            Lost and Found Pets
          </h1>
          <p class="text-gray-500 dark:text-gray-400">
            Report a missing pet or help reunite lost pets with their owners.
          </p>
          <div class="flex">
            <UInput class="mt-5 w-96" placeholder="Enter your location" />
            <UButton
              color="primary"
              class="mt-5 ml-2 px-4"
              @click="() => $router.push('/pets')"
              >Search</UButton
            >
          </div>
        </div>
        <img
          src="https://images.unsplash.com/photo-1629740067905-bd3f515aa739?q=80&w=1888&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          width="600"
          height="300"
          alt="Hero"
          class="aspect-[2/1] h-[450px] rounded-lg overflow-hidden object-cover object-center"
        />
      </div>
    </div>
  </section>
</template>
