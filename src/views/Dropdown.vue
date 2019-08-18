<template>
  <div class="h-screen flex items-center justify-center">
    <div class="absolute top-0 left-0 p-8">
      <router-link
        to="/"
        class="font-semibold text-blue-500 hover:text-green-500 focus:outline-none"
      >
        Back to Home
      </router-link>
    </div>
    <dropdown-menu classes="w-full">
      <template v-slot:trigger>
        <button class="font-semibold text-blue-500 hover:text-green-500 focus:outline-none">
          Example With Full Width Menu
        </button>
      </template>

      <li>
        <a
          href="#"
          class="pl-2 pr-8 leading-loose text-xs block hover:bg-gray-900"
        >Edit</a>
      </li>
      <li><a
          href="#"
          class="pl-2 pr-8 leading-loose text-xs block hover:bg-gray-900"
        >Delete</a></li>
      <li><a
          href="#"
          class="pl-2 pr-8 leading-loose text-xs block hover:bg-gray-900"
        >Report</a></li>
    </dropdown-menu>
  </div>
</template>

<script>
import DropdownMenu from '@/components/DropdownMenu.vue';

export default {
  components: {
    DropdownMenu,
  },
};
</script>
