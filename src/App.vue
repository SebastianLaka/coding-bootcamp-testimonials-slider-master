<script setup>
import fontsComponent from './components/fonts-component.vue'
import tanyaComponent from './components/tanya-component/woman-card-component.vue'
import johnComponent from './components/john-component/john-card-component.vue'
import { ref } from 'vue';

const countSlide = ref(0);

</script>
<template>
  <fontsComponent />
  <tanyaComponent  />
  <johnComponent  />
</template>

<style lang="scss">
@use '@/assets/scss/responsive-styles/media-queries.scss' as *;
</style>
