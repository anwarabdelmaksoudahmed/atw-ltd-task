<script setup>
import IconLayers from '../assets/icons/layers.svg';
import IconShow from '../assets/icons/show.svg';

const props = defineProps(['title', 'image']);
</script>

<template>
  <div class="image-card-wrapper">
    <img class="image-card-image" :src="props.image" alt="" />

    <h4 class="image-card-title">{{ props.title }}</h4>

    <div class="image-card-actions">
      <div class="action">
        <img :src="IconLayers" />
        <span>View Study Case</span>
      </div>

      <div class="action">
        <img :src="IconShow" />
        <span>Live Preview</span>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.image-card {
  &-wrapper {
    margin-bottom: 100px;
    padding: 0 15px;
  }

  &-image {
    border-radius: 25px;
    width: 100%;
    height: 380px;
    flex-shrink: 0;
    margin-bottom: 30px;
    object-fit: cover;
  }

  &-title {
    color: var(--1-c-1-c-1-c, #1c1c1c);
    font-family: Poppins;
    font-size: 24px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }

  &-actions {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    .action {
      color: #151517;
      line-height: normal;
      display: flex;
      align-items: center;

      &:not(:last-child) {
        margin-right: 50px;
      }

      img {
        width: 20px;
        height: 20px;
        margin-right: 13px;
      }
    }
  }
}
</style>
