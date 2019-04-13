<template>
  <router-link to="/" class="close-button">
    <span></span>
  </router-link>
</template>

<style lang="scss" scoped>
.close-button {
  display: inline-block;
  width: 8rem;
  height: 8rem;
  position: relative;
  border: 1px solid rgba(0, 0, 0, 0.1);
  background-color: rgba(172, 164, 164, 0.9);
  box-shadow: 3px 3px 3px 3px rgba(0, 0, 0, 0.3);
  margin-left: 80%;
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
@media (max-width: 767px) {
  .close-button {
    width: 5.5rem;
    height: 5.5rem;
    margin-left: 68%;
  }
}
</style>
