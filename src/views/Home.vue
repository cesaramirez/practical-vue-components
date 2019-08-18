<template>
  <div class="h-screen flex flex-col items-center justify-center">
    <div class="flex items-center justify-center">
      <h1 class="text-5xl tracking-wide font-bold text-center">
        Practical Vue Components
      </h1>
    </div>
    <img
      alt="Vue logo"
      class="h-40 w-40"
      src="@/assets/logo.png"
    />
    <ul class="text-center mt-16">
      <li class="text-blue-500 hover:text-green-500 tracking-wide font-bold text-lg">
        <router-link to="/smooth">Smooth Scrolling</router-link>
      </li>
      <li class="text-blue-500 hover:text-green-500 tracking-wide font-bold text-lg">
        <router-link to="/dropdown">Dropdown Menu</router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'home',
};
</script>
