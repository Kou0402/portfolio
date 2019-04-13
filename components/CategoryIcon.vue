<template>
  <router-link :to="linkName" class="category-icon">
    <span>
      <slot></slot>
    </span>
  </router-link>
</template>

<script>
export default {
  props: {
    linkName: {
      type: String,
      default: '/'
    }
  }
}
</script>

<style lang="scss" scoped>
.category-icon {
  background-color: rgba(157, 177, 202, 1);
  position: relative;
  width: 50%;
  height: 50%;
  padding: 25%;
  border-radius: 50%;
  margin: auto;
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
    font-size: 3rem;
  }
}
@media (max-width: 767px) {
  .category-icon {
    span {
      font-size: 2rem;
    }
  }
}
</style>
