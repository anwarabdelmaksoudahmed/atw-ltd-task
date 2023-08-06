<script setup>
import IconInstagram from '../assets/icons/instagram.svg';
import IconYoutube from '../assets/icons/youtube.svg';
import IconDribble from '../assets/icons/dribbble.svg';
import IconArrowUp from '../assets/icons/short_up.svg';
</script>

<template>
  <footer>
    <div class="section">Let's Connect</div>

    <div class="section social">
      <img :src="IconInstagram" />
      <img :src="IconYoutube" />
      <img :src="IconDribble" />
    </div>

    <div class="section">
      <span>Back to Top</span>
      <img :src="IconArrowUp" />
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 59px;

  .section {
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;

    &:first-child {
      justify-content: flex-start;
      color: #2f2f2f;
      font-size: 36px;
      line-height: 46px;
    }

    &:last-child {
      justify-content: flex-end;
      color: #2f2f2f;
      font-size: 24px;
      line-height: 36px;

      img {
        width: 18px;
        height: 24px;
        margin-left: 13px;
      }
    }

    &.social {
      img {
        width: 32px;
        height: 32px;
        margin-right: 25px;
      }
    }
  }
}
</style>
