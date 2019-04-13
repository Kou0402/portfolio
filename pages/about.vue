<template>
  <section>
    <div class="wrapper">
      <CloseButton class="close-button"></CloseButton>
      <article>
        <h2>about</h2>
        <p>2013年 都内某4年制大学経済学部に入学</p>
        <p>2016年 専門商社の営業職に新卒入社。</p>
        <p>2017年 退職。</p>
        <p>2017年 訓練校にてプログラミング学習(Java)。</p>
        <p>2018年 SIerに入社しSEに転職。</p>
      </article>
    </div>
  </section>
</template>

<script>
import CloseButton from '~/components/CloseButton.vue'

export default {
  components: {
    CloseButton
  }
}
</script>

<style scoped lang="scss">
section {
  .wrapper {
    background-color: rgba(157, 177, 202, 0.37);
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    position: absolute;
    margin: auto;
    .close-button {
      margin-left: 85rem;
    }
    article {
      padding: 3rem 15rem;
      color: rgb(172, 164, 164);
      h2 {
        font-size: 4rem;
        text-decoration: underline;
        letter-spacing: 2rem;
      }
      p {
        margin: 3.2rem 4rem;
        letter-spacing: 0.9rem;
        font-size: 2rem;
      }
    }
  }
  @media (max-width: 767px) {
    .wrapper {
      width: 25rem;
    }
  }
  @media (min-width: 768px) {
    .wrapper {
      width: 75%;
      height: 70%;
      border-radius: 50%;
    }
  }
}
</style>
