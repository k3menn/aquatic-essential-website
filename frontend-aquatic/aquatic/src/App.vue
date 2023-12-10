<script setup>
import Header  from './components/Layout/Header.vue';
import Carousel from './components/Сarousel.vue';
</script>

<template>
  <div class="container">
    <Header/>
    <Carousel/>
  </div>
</template>

<style scoped>

* {
  box-sizing: border-box;
}

body{
  margin: 0;
  padding: 0;
  font-family: 'Montserrat', sans-serif;
  color: #FFFFFF;
}

img {
  width: 100%;
}
.container{
  /* font-family: 'Montserrat', sans-serif; */
  max-width: 1920px;
  margin: auto;
}
</style>
