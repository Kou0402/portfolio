<template>
  <router-link to="/" class="close-button">
    <span></span>
  </router-link>
</template>

<style lang="scss" scoped>
.close-button {
  width: 6.5rem;
  height: 6.5rem;
  position: absolute;
  background-color: rgba(255, 255, 255, 0.2);
  top: -3.5rem;
  right: -3.5rem;
  cursor: pointer;
  &:hover {
    background-color: rgba(255, 255, 255, 0.8);
  }
  &:before,
  &:after {
    display: block;
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 130%;
    height: 2%;
    margin: 0 0 0 -64%;
    background: rgb(0, 0, 0);
  }
  &:before {
    transform: rotate(-45deg);
  }
  &:after {
    transform: rotate(45deg);
  }
}
</style>
