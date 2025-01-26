<template>
    <div class="pb-16 bg-gray-50">
      <div class="max-w-7xl mx-auto px-4">
        <!-- Section Heading -->
        <div class="text-center mb-12">
          <h2 class="text-3xl font-bold text-blue-600">
            Key <span class="text-gray-900">Features</span> of HRM
          </h2>
          <p class="text-gray-500 mt-2">
            Our customers love us, and we know you will too.
          </p>
        </div>
  
        <!-- Features Grid -->
        <div class="grid grid-cols-1 md:grid-cols-1 gap-12">
          <div
            v-for="(feature, index) in features"
            :key="index"
            :class="[
              'flex flex-col gap-6 items-center',
              index % 2 === 0 ? 'md:flex-row' : 'md:flex-row-reverse'
            ]"
          >
            <!-- Feature Image -->
            <img
              :src="feature.image"
              :alt="feature.title"
              class="w-full md:w-1/2 rounded-lg "
            />
            <!-- Feature Content -->
            <div class="md:w-1/2">
              <h3 class="text-xl font-bold text-gray-800 mb-4">
                {{ feature.title }}
              </h3>
              <p class="text-gray-600 mb-4">{{ feature.description }}</p>
              <button class="inline-flex items-center px-6 py-2 border border-blue-600 text-blue-600 font-medium rounded-lg hover:bg-blue-600 hover:text-white transition">
                Learn More
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-5 w-5 ml-2"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import process from "/assets/css/img/1.png"
  export default {
    data() {
      return {
        features: [
          {
            title: "Task Management Dashboard",
            description:
              "The Task Management feature allows users to create, assign, track, and manage tasks efficiently within the HRM software. With a clear overview of all active, completed, and pending tasks, employees and managers can stay organized, prioritize responsibilities, and meet deadlines seamlessly. Tasks can be categorized, assigned to team members, and monitored through a simple, intuitive interface for optimal productivity.",
            image: process,
          },
          {
            title: "More Applicants. Less Wasted Time.",
            description:
              "With LuminoHR, all your employee information lives in a single, secure database, with powerful reporting tools and seamless editing capabilities at your fingertips. Managing workforce data has never been easier, faster, or more accurate, and the road to exceptional HR has never been this clear.",
            image: process,
          },
          {
            title: "Hire the Best in Less Time.",
            description:
              "With LuminoHR, all your employee information lives in a single, secure database, with powerful reporting tools and seamless editing capabilities at your fingertips. Managing workforce data has never been easier, faster, or more accurate, and the road to exceptional HR has never been this clear.",
            image: process,
          },
          {
            title: "Hire the Best in Less Time.",
            description:
              "With LuminoHR, all your employee information lives in a single, secure database, with powerful reporting tools and seamless editing capabilities at your fingertips. Managing workforce data has never been easier, faster, or more accurate, and the road to exceptional HR has never been this clear.",
            image: process,
          },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  /* You can add custom styles here if needed */
  </style>
  