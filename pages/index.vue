<template>
  <div class="">
    <navbar />
    <hero-section />
    <div class="mt-12">
      <div class="text-center">
        <h1
          class="text-3xl font-bold tracking-tighter sm:text-2xl md:text-3xl xl:text-4xl/none"
        >
          Help find lost pets or register a lost pet.
        </h1>
        <p class="text-gray-500 dark:text-gray-400 mt-4">
          We will do our best to spread the word to try to find your beloved
          pet.
        </p>
      </div>
      <div class="flex justify-center">
        <filters class="" />
      </div>
      <div class="flex justify-around flex-wrap">
        <card
          title="Pandora"
          description="A golden retriever lost in Central Park"
          location="Central Park"
          image="https://source.unsplash.com/random/?Dog&1"
          type="Dog"
          class="mt-6"
        />
        <card
          title="Pandora"
          description="A golden retriever lost in Central Park"
          location="Central Park"
          image="https://source.unsplash.com/random/?Dog&2"
          type="Dog"
          class="mt-6"
        />
        <card
          title="Pandora"
          description="A golden retriever lost in Central Park"
          location="Central Park"
          image="https://source.unsplash.com/random/?Dog&3"
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
    <div class="flex items-center justify-center mt-12">
      <UPagination
        v-model="page"
        :total="totalPets"
        :page-count="9"
        @update:model-value="fetchPets"
      />
    </div>
  </div>
  <footer-missing class="mt-12" />
</template>

<script setup lang="ts">
import Navbar from "~/components/Navbar.vue";
import HeroSection from "~/components/HeroSection.vue";
import Card from "~/components/Card.vue";
import FooterMissing from "~/components/FooterMissing.vue";

import { onMounted, ref } from "vue";

interface Pet {
  title: string;
  description: string;
  location: string;
  image: string;
  type: string;
}

interface PetResponse {
  data: Pet[];
  total: number;
}

const pets = ref<Pet[]>();
const totalPets = ref<number>(0);
const page = ref<number>(1);

const fetchPets = async (page: number) => {
  fetch(`https://www.ejsocial.com/api/pet/posts?page=${page}`, {
    method: "GET",
    headers: {
      "Content-Type": "application/json",
    },
  }).then((response) => {
    response.json().then((data: PetResponse) => {
      pets.value = data.data;
      totalPets.value = data.total;
    });
  });
};

onMounted(() => {
  fetchPets(1);
});
</script>
