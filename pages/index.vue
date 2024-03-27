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
          v-for="pet in pets"
          :key="pet.id"
          v-bind="pet"
          :title="pet.breed"
          :description="pet.additional_info"
          location="Central Park"
          :image="
            'https://source.unsplash.com/random/470x380/?' +
            pet.type +
            '&' +
            pet.id
          "
          :type="pet.type"
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
  id: number;
  breed: string;
  additional_info: string;
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
      pets.value = data.data.map((pet) => {
        return { ...pet, type: pet.id % 2 === 0 ? "Dog" : "Cat" };
      });
      totalPets.value = data.total;
    });
  });
};

onMounted(() => {
  fetchPets(1);
});
</script>
