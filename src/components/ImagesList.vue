<script setup>
import { ref } from 'vue'
import ImageItem from './ImageItem.vue'
import galleryData from '../assets/data.json'

const data = ref(galleryData)
console.log(data)
</script>

<template>
  <section class="gallery">
    <ImageItem v-for="item in data" :key="item.name" :item="item" />
  </section>
</template>
<style scoped>
.gallery {
  max-width: 1440px;
  width: 100%;
  margin: 0 auto;
  padding: 40px;
  column-count: 4;
  gap: 40px;
}
@media (max-width: 1024px) {
  .gallery {
    max-width: 1024px;
    column-count: 3;
  }
}
@media (max-width: 768px) {
  .gallery {
    max-width: 768px;
    column-count: 2;
  }
}

@media (max-width: 500px) {
  .gallery {
    max-width: 375px;
    column-count: 1;
    padding: 24px;
    gap: 24px;
  }
}
</style>
