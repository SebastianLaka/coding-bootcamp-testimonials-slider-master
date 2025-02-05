<script setup>
import fontsComponent from './components/fonts-component.vue'
import tanyaComponent from './components/tanya-component/woman-card-component.vue'
import johnComponent from './components/john-component/john-card-component.vue'
import { onMounted } from 'vue';

onMounted(() => {
  const buttons = document.querySelectorAll('.buttons-area__slider-btn');

  buttons.forEach(button => {
    button.addEventListener('click', (event) => {
      console.log('Clicked!', event.target);
    });
  });
});
</script>
<template>
  <fontsComponent />
  <tanyaComponent />
  <johnComponent />
</template>

<style lang="scss">
@use '@/assets/scss/responsive-styles/media-queries.scss' as *;
</style>
