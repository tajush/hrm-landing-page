<template>
    <section :style="{ backgroundImage: `url(${image})` }"
      class="relative  bg-cover bg-center bg-no-repeat h-screen flex items-center justify-center text-center"
    >
      <div class=" inset-0 bg-black bg-opacity-60"></div>
      <div class="relative z-10 max-w-2xl text-white">
        <h1 class="text-4xl md:text-5xl font-bold mb-4">
          Start making great hires today.
        </h1>
        <p class="text-lg mb-6">
          Try LuminoHR for free - no credit card required - to see how easy it is to streamline and improve your entire recruiting process.
        </p>
        <button class="bg-yellow-500 cursor-pointer text-black font-semibold py-2 px-6 rounded hover:bg-yellow-600 transition">
          Contact Us
        </button>
      </div>
    </section>
  </template>
  
  <script>
  // Correct image import using the path directly
  import footer_bg from 'assets/css/img/Savoir.png';
  
  export default {
    name: 'CallToAction',
    data() {
      return {
        image: footer_bg, // Image is now assigned properly
      };
    },
  };
  </script>
  
  <style scoped>
  /* Add any additional custom styles here */
  </style>
  