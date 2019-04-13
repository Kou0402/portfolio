<template>
  <router-link to="/" class="close-button-wrapper">
    <span></span>
  </router-link>
</template>

<style lang="scss" scoped>
.close-button-wrapper {
  display: inline-block;
  width: 9rem;
  height: 9rem;
  position: relative;
  border: 1px solid rgba(0, 0, 0, 0.1);
  background-color: rgb(172, 164, 164);
  cursor: pointer;
  &:before,
  &:after {
    display: block;
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 130%;
    height: 2%;
    margin: -2% 0 0 -64%;
    background: rgba(40, 56, 94, 1);
  }
  &:before {
    transform: rotate(-45deg);
  }
  &:after {
    transform: rotate(45deg);
  }
}
</style>
