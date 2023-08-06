<template>
  <div>
    <h2>Our <br />Projects</h2>

    <ul>
      <li class="active">Web Design</li>
      <li>Mobile App Design</li>
      <li>Freebies</li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
h2 {
  color: #000;
  font-size: 48px;
  font-style: normal;
  font-weight: 600;
  line-height: 62px;
  margin-bottom: 40px;
}
ul {
  display: flex;
  align-items: center;
  list-style: none;
  padding: 0;

  li {
    color: #828282;
    font-size: 32px;
    font-style: normal;
    font-weight: 600;
    line-height: 54px;
    padding-bottom: 12px;
	cursor: pointer;

    &.active {
      color: #eebf63;
      border-bottom: 5px solid #eebf63;
    }

    &:not(:last-child) {
      margin-right: 80px;
    }
  }
}
</style>
