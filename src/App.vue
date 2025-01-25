<script setup>

</script>

<template>
  <div>
    <p>Test</p>
  </div>
</template>

<style scoped lang="scss">
body{
  div{
    @include flex;
    background-color: $red;
    p{
      color: $blue;
    }
  }
}
</style>
