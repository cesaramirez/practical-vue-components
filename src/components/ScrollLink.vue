<template>
  <a :href="href" @click.prevent="scroll">
    <slot></slot>
  </a>
</template>

<script>
import smoothscroll from 'smoothscroll-polyfill';

export default {
  props: ['href'],
  mounted() {
    smoothscroll.polyfill();
  },
  methods: {
    scroll() {
      document.querySelector(this.href).scrollIntoView({ behavior: 'smooth' });
    },
  },
};
</script>
