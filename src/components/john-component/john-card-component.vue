<template>
  <div class="card-component">
    <div class="card-image-area">
      <!-- <img src="../icons/pattern-bg.svg" alt="" class="card-image-area__bg-img" /> -->
      <img src="../icons/image-john.jpg" alt="Tanya image" class="card-image-area__image" />
      
      <div class="buttons-area">
        <button @click="$emit('slide', 'left')" class="buttons-area__button-left"><img src="../icons/icon-prev.svg" alt="Button right in slider"></button>
        <button @click="$emit('slide', 'right')" class="buttons-area__button-right"><img src="../icons/icon-next.svg" alt="Button left in slider"></button>
        
      </div>
    </div>
    <div class="card-description">
      <p class="card-description__about-person">
        “ If you want to lay the best foundation possible I’d recommend taking this course. The depth the instructors go into is incredible. I now feel so confident about starting up as a professional developer. ”
      </p>
      <div class="card-person-signature">
        <p class="card-person-signature__person-name">John Trakpor</p>
        <p class="card-person-signature__person-job">Junior Front-end Developer</p>
      </div>
    </div>
  </div>
</template>
<script setup>
import { defineEmits } from 'vue';
const emit = defineEmits(['slide']);
</script>
