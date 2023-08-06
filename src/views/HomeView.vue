<script setup>
import HomeHeader from '../components/HomeHeader.vue';
import ImageCard from '../components/ImageCard.vue';
import NotifyPanel from '../components/NotifyPanel.vue';
import Footer from '../components/Footer.vue';

import Image1 from '../assets/images/image_1.png';
import Image2 from '../assets/images/image_2.jpeg';
import Image3 from '../assets/images/image_3.jpeg';
import Image4 from '../assets/images/image_4.jpeg';
</script>

<template>
  <main class="container">
    <div class="header-wrapper">
      <HomeHeader />
    </div>

    <div class="image-cards">
      <ImageCard title="Minify - Web Design" :image="Image1" />
      <ImageCard title="Ant - Personal Portofolio" :image="Image2" />
      <ImageCard title="Lumy - Dashboard UI Kit" :image="Image3" />
      <ImageCard title="Keeper - Soccer Site" :image="Image4" />
    </div>

    <section class="panel">
      <NotifyPanel />
    </section>

    <Footer />
  </main>
</template>

<style lang="scss" scoped>
.header-wrapper {
  margin-bottom: 62px;
}

.image-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;

  .image-card-wrapper {
    width: 50%;
  }
}

.panel {
  margin-bottom: 100px;
}
</style>
