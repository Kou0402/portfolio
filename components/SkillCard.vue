<template>
  <article class="skill-card">
    <img :src="filePath" class="image" />
    <div class="star">{{ star }}</div>
  </article>
</template>

<script>
export default {
  props: {
    fileName: {
      type: String,
      default: ''
    },
    star: {
      type: String,
      default: ''
    }
  },
  data() {
    return {
      filePath: require('~/assets/img/' + this.fileName)
    }
  }
}
</script>

<style scoped lang="scss">
.skill-card {
  width: 16rem;
  height: 12rem;
  text-align: center;
  margin: 0 1.4vw;
  .image {
    width: auto;
    height: 7rem;
  }
  .star {
    margin: 1rem;
  }
}
@media screen and (max-width: 896px) {
  .skill-card {
    width: 8rem;
    height: 9rem;
    margin: 0 1.8vw;
    .image {
      width: auto;
      height: 4rem;
    }
    .star {
      margin: 1rem;
    }
  }
}
</style>
