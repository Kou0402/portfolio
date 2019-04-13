<template>
  <router-link to="about" class="router-link">
    <span>
      <slot></slot>
    </span>
  </router-link>
</template>

<style lang="scss" scoped>
.router-link {
  background-color: rgba(157, 177, 202, 1);
  position: relative;
  width: 50%;
  height: 50%;
  padding: 25%;
  border-radius: 50%;
  margin: 1em;
  box-shadow: 3px 3px 3px 3px rgba(0, 0, 0, 0.3);
  display: block;
  span {
    position: absolute;
    left: 0;
    top: 50%;
    margin: -0.5em 0 0;
    width: 100%;
    text-align: center;
    color: rgba(40, 56, 94, 1);
    @media (max-width: 767px) {
      font-size: 2rem;
    }
    @media (min-width: 768px) {
      font-size: 3rem;
    }
  }
}
</style>
