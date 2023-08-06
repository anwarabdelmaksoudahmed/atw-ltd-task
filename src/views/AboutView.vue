<script setup>
import { onMounted, ref } from 'vue';
import ImageCard from '../components/ImageCard.vue';
import Footer from '../components/Footer.vue';

let images = ref([]);

const getImages = () => {
  return fetch('https://jsonplaceholder.typicode.com/photos?albumId=100')
    .then((res) => res.json())
    .then((data) => {
      images.value.push(...data);

      console.log(data);
    });
};

onMounted(() => {
  getImages();
});
</script>

<template>
  <main class="container">
    <div class="image-cards">
      <ImageCard v-for="image in images" :key="image.id" :title="image.title" :image="image.thumbnailUrl" />
    </div>

    <Footer />
  </main>
</template>

<style lang="scss" scoped>
.image-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;

  .image-card-wrapper {
    width: 50%;
  }
}
</style>
