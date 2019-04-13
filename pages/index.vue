<template>
  <main>
    <h1 class="main-title">welcome</h1>
    <div class="row">
      <article class="project">
        <CategoryIcon class="category-icon">project</CategoryIcon>
      </article>
      <article class="product">
        <CategoryIcon class="category-icon">product</CategoryIcon>
      </article>
    </div>
    <div class="row">
      <article class="about">
        <CategoryIcon class="category-icon">about</CategoryIcon>
      </article>
    </div>
    <div class="row">
      <article class="skill">
        <CategoryIcon class="category-icon">skill</CategoryIcon>
      </article>
      <article class="sns">
        <CategoryIcon class="category-icon">sns</CategoryIcon>
      </article>
    </div>
  </main>
</template>

<script>
import CategoryIcon from '~/components/CategoryIcon.vue'

export default {
  components: {
    CategoryIcon
  }
}
</script>

<style scoped lang="scss">
main {
  margin-top: 5%;
  .main-title {
    position: absolute;
    font-size: 7rem;
    letter-spacing: 2rem;
    color: rgba(196, 196, 196, 1);
    top: 18%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .row {
    display: flex;
    position: relative;
    height: 25rem;
    article {
      position: absolute;
      .category-icon {
        margin: auto;
      }
    }
    .project {
      left: 14rem;
      top: 13rem;
    }
    .product {
      right: 13rem;
      top: 10rem;
    }
    .about {
      position: relative;
      margin: auto;
    }
    .skill {
      left: 7rem;
      bottom: 13rem;
    }
    .sns {
      right: 21rem;
      bottom: 10rem;
    }
    @media (max-width: 767px) {
      article {
        width: 25rem;
      }
    }
    @media (min-width: 768px) {
      article {
        width: 37rem;
      }
    }
  }
}
</style>
