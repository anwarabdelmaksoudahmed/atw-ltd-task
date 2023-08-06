<script setup>
import { RouterLink } from 'vue-router';
</script>

<template>
  <nav>
    <div class="container inner">
      <h1>LOGO</h1>
      <ul>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/project">Project</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </ul>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
nav {
  width: 100%;
  height: 100px;
  padding: 2rem;

  @media screen and (max-width: 768px) {
    padding: 1.5rem 165px 1.5rem 165px;
  }

  .inner {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  h1 {
    color: #151517;
    font-size: 22px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
  }

  ul {
    a {
      color: #2f2f2f;
      text-align: center;
      font-size: 1rem;
      font-style: normal;
      font-weight: 500;
      line-height: normal;
      text-decoration: none;

      &:not(:last-child) {
        margin-right: 40px;
      }

      &.router-link-active {
        color: #eebf63;
        font-weight: 700;
      }
    }
  }
}
</style>
