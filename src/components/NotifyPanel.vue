<script setup>
import IconMail from '../assets/icons/mail.svg';
</script>

<template>
  <div class="notify-panel-wrapper">
    <div class="left">
      <h1>Interested working with me?</h1>
    </div>

    <div class="right">
      <button>
        <img :src="IconMail" />
        <span>Email Me</span>
      </button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.notify-panel-wrapper {
  display: flex;
  justify-content: space-between;
  padding: 50px 75px;
  border-radius: 25px;
  background-color: #eebf63;

  .left,
  .right {
    flex: 1 1 50%;
  }

  h1 {
    color: white;
    font-family: Poppins;
    font-size: 48px;
    font-style: normal;
    font-weight: 600;
    line-height: 62px;
  }

  .right {
    display: flex;
    align-items: center;
    justify-content: flex-end;

    button {
      height: 70px;
      border-radius: 10px;
      width: 259px;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: white;
      box-shadow: 0px 0.9274210333824158px 1.9235398769378662px 0px rgba(0, 0, 0, 0.01);
      color: #2f2f2f;
      border: none;
      outline: none;

      span {
        font-size: 24px;
        font-weight: 600;
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
