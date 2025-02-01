<script setup>
import fontsComponent from './components/fonts-component.vue';
import tanyaComponent from './components/tanya-component/woman-card-component.vue';
import johnCardComponent from './components/john-component/john-card-component.vue';
</script>

<template>
  <fontsComponent />
  <tanyaComponent />
  <!-- <johnCardComponent/> -->
</template>

<style lang="scss">
@use '@/assets/scss/responsive-styles/media-queries.scss' as *;
</style>
