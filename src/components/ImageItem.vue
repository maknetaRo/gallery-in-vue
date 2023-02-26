<script setup>
const props = defineProps({
  item: Object
})
</script>

<template>
  <figure>
    <img class="gallery-img" :src="item.images.gallery" alt="" />
    <figcaption>
      <h3 class="art-title">{{ item.name }}</h3>
      <h4 class="art-author">{{ item.artist.name }}</h4>
    </figcaption>
  </figure>
</template>
<style scoped>
figure {
  max-width: 310px;
  width: 100%;
  height: 100%;
  display: flex;
  flex-flow: column;
  position: relative;
  margin-bottom: 40px;
}
.gallery-img {
  width: 100%;
  min-height: 250px;
  height: 100%;
  object-fit: cover;
}
figcaption {
  padding: 3px;
  background: rgba(0, 0, 0, 0.5);
  position: absolute;
  color: white;
  bottom: 0px;
  left: 0px;
  width: 100%;
  padding: 32px;
  padding-top: 16px;
}
.art-title {
  font-size: 24px;
  line-height: 30px;
  font-weight: 30px;
  max-width: 246px;
}
.art-author {
  font-size: 13px;
  line-height: 16px;
  opacity: 0.75;
  max-width: 246px;
}
@media (max-width: 376px) {
  figure {
    max-width: 327px;
  }
}
</style>
