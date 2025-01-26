<script setup>
import fontsComponent from './components/fonts-component.vue';
</script>

<template>
<fontsComponent/>
  <div class="root">
    <div class="test1">
      <h1>header 1</h1>
      <p>Test</p>
    </div>
    <div class="test1">
      <p>Test</p>
    </div>
    <div class="test1">
      <p>Test</p>
    </div>
  </div>
</template>

<style lang="scss">
@use '@/assets/scss/responsive-styles/media-queries.scss' as *;
</style>
