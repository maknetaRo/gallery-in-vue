<script setup>
import NavBar from '@/components/NavBar.vue'
import ImagesList from '@/components/ImagesList.vue'
</script>

<template>
  <NavBar />
  <main class="main">
    <ImagesList />
  </main>
</template>

<style scoped>
.main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  max-width: 1440px;
  width: 100%;
  margin: 0 auto;
}
</style>
