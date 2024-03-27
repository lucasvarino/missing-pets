<template>
  <div class="">
    <navbar />
    <hero-section />
    <div class="mt-12 text-center">
      <h1
        class="text-3xl font-bold tracking-tighter sm:text-2xl md:text-3xl xl:text-4xl/none"
      >
        Help find lost pets or register a lost pet.
      </h1>
      <p class="text-gray-500 dark:text-gray-400 mb-12 mt-4">
        We will do our best to spread the word to try to find your beloved pet.
      </p>
      <div class="flex justify-center">
        <filters class="" />
      </div>
      <div class="flex justify-around flex-wrap">
        <card
          title="Pandora"
          description="A golden retriever lost in Central Park"
          location="Central Park"
          image="https://images.unsplash.com/photo-1591160690555-5debfba289f0?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8Z29sZGVuJTIwcmV0cmlldmVyfGVufDB8fDB8fHww"
          type="Dog"
          class="mt-6"
        />
        <card
          title="Pandora"
          description="A golden retriever lost in Central Park"
          location="Central Park"
          image="https://images.unsplash.com/photo-1591160690555-5debfba289f0?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8Z29sZGVuJTIwcmV0cmlldmVyfGVufDB8fDB8fHww"
          type="Dog"
          class="mt-6"
        />
        <card
          title="Pandora"
          description="A golden retriever lost in Central Park"
          location="Central Park"
          image="https://images.unsplash.com/photo-1591160690555-5debfba289f0?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8Z29sZGVuJTIwcmV0cmlldmVyfGVufDB8fDB8fHww"
          type="Dog"
          class="mt-6"
        />
        <card
          title="Pandora"
          description="A golden retriever lost in Central Park"
          location="Central Park"
          image="https://images.unsplash.com/photo-1591160690555-5debfba289f0?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8Z29sZGVuJTIwcmV0cmlldmVyfGVufDB8fDB8fHww"
          type="Dog"
          class="mt-6"
        />
      </div>
    </div>
  </div>
</template>

<script setup>
import Navbar from "~/components/Navbar.vue";
import HeroSection from "~/components/HeroSection.vue";
import Card from "~/components/Card.vue";
</script>
