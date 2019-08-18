<template>
  <div class="p-8">
    <h1 class="text-3xl font-bold">Smooth Scroll</h1>
    <ul>
      <li>
        <router-link
          to="/"
          class="text-blue-500 hover:text-green-500 font-semibold"
        >
          Back to Home
        </router-link>
      </li>
      <li>
        <scroll-link
          href="#categories"
          class="text-blue-500 hover:text-green-500 font-semibold"
        >
          Go To Testimonials
        </scroll-link>
      </li>
    </ul>
    <div style="height: 2000px"></div>
    <div id="categories">
      <h2 class="font-bold mb-6">Testimonials</h2>
      <div class="flex flex-col md:flex-row">
        <div class="w-full md:w-1/3 h-32 md:h-48 bg-gray-200 p-4">
          <scroll-link
            href="#app"
            class="font-semibold text-blue-500 hover:text-green-500"
          >
            Go Back Up
          </scroll-link>
        </div>
        <div class="w-full md:w-1/3 h-32 md:h-48 bg-gray-400 p-4">Item</div>
        <div class="w-full md:w-1/3 h-32 md:h-48 bg-gray-200 p-4">Item</div>
      </div>
    </div>
  </div>
</template>

<script>
import ScrollLink from '@/components/ScrollLink.vue';

export default {
  name: 'Smooth',
  components: {
    ScrollLink,
  },
};
</script>
