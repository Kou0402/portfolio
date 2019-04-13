<template>
  <main>
    <h1 class="main-title">welcome</h1>
    <div class="row">
      <article class="project">
        <CategoryIcon>project</CategoryIcon>
      </article>
      <article class="product">
        <CategoryIcon>product</CategoryIcon>
      </article>
    </div>
    <div class="row">
      <article class="about">
        <CategoryIcon link-name="about">about</CategoryIcon>
      </article>
    </div>
    <div class="row">
      <article class="skill">
        <CategoryIcon>skill</CategoryIcon>
      </article>
      <article class="sns">
        <CategoryIcon>sns</CategoryIcon>
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
  .main-title {
    position: absolute;
    font-size: 4.5vw;
    letter-spacing: 2rem;
    color: rgba(196, 196, 196, 1);
    top: 15%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .row {
    display: flex;
    position: relative;
    height: 25rem;
    article {
      position: absolute;
    }
    @media (max-width: 767px) {
      article {
        width: 24rem;
      }
      .project {
        left: 0%;
        top: 73%;
      }
      .product {
        right: 0%;
        top: 68%;
      }
      .about {
        position: relative;
        margin: 20% auto;
      }
      .skill {
        left: 0%;
        bottom: 50%;
      }
      .sns {
        right: 0%;
        bottom: 55%;
      }
    }
    @media (min-width: 768px) {
      article {
        width: 35rem;
      }
      .project {
        left: 13%;
        top: 68%;
      }
      .product {
        right: 13%;
        top: 70%;
      }
      .about {
        position: relative;
        margin: 8% auto;
      }
      .skill {
        left: 8%;
        bottom: 30%;
      }
      .sns {
        right: 10%;
        bottom: 30%;
      }
    }
  }
}
</style>
