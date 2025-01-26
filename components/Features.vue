<script setup>
import { ref } from 'vue';
// Import your SVG image
import users from '/assets/css/img/users.svg';
import rocket from '/assets/css/img/rocket.svg';
import data from '/assets/css/img/data-icon.svg';
// Define the features array
const features = ref([
  {
    id: 1,
    icon: users, // Use the image path here
    title: 'Unlimited jobs & users.',
    description:
      'Say goodbye to pay-per-user and limited channels. Enjoy unlimited access without extra fees or costs.',
    link: '#',
  },
  {
    id: 2,
    icon: rocket, // Use the image path here
    title: 'Recruit better and Faster.',
    description:
      'Our platform simplifies the hiring process, saving you time and letting you focus on the human side of recruiting.',
    link: '#',
  },
  {
    id: 3,
    icon: data, // Use the image path here
    title: 'People Data & Analytics.',
    description:
      'Our software empowers you to create customized solutions tailored to your hiring needs with powerful analytics.',
    link: '#',
  },
]);
</script>

<template>
  <section class="pb-16 bg-gray-50">
    <div class="max-w-7xl text-center mx-auto px-4">
      <!-- Section Heading -->
      <h2 class="text-3xl font-bold text-gray-900 mb-4">
        How can we <span class="text-blue-500">help</span> you get started?
      </h2>
      <p class="text-gray-600 mb-12">
        Our customers love us, and we know you will too.
      </p>

      <!-- Features Grid -->
      <div class="grid  grid-cols-1 md:grid-cols-3 gap-8">
        <div
          v-for="feature in features"
          :key="feature.id"
          class="flex flex-col  hover:shadow-2xl transition-shadow duration-300 p-6 bg-white   items-center text-center   shadow-md rounded-md"
        >
          <div class="mb-4">
            <!-- Render the icon as an image -->
            <img :src="feature.icon" alt="Feature Icon" class="w-12 h-12 text-blue-500" />
          </div>
          <h3 class="text-xl font-semibold text-gray-800 mb-2">
            {{ feature.title }}
          </h3>
          <p class="text-gray-600 mb-4">{{ feature.description }}</p>
          <a :href="feature.link" class="text-blue-500 font-medium hover:underline">
            Learn More
          </a>
        </div>
      </div>
    </div>
  </section>
</template>
