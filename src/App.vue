<script setup>
import fontsComponent from './components/fonts-component.vue'
import tanyaComponent from './components/tanya-component/woman-card-component.vue'
import johnComponent from './components/john-component/john-card-component.vue'
import { ref } from 'vue';

const currSlide = ref(0);
const slidesCount = 2;

const slideRight = () => {
    currSlide.value = (currSlide.value - 1 + slidesCount) % slidesCount;
}
const slideLeft = () =>{
  currSlide.value = (currSlide.value + 1) % slidesCount;
}
const slider = () =>{
  if(currSlide.value === 0){
    slideRight()
  }else{
    slideLeft()
  }
}
slider();
</script>
<template>
  <fontsComponent />
  <tanyaComponent v-if="currSlide === 1" @slide="slider" />
  <johnComponent v-if="currSlide === 0" @slide="slider" />
</template>

<style lang="scss">
@use '@/assets/scss/responsive-styles/media-queries.scss' as *;

</style>
