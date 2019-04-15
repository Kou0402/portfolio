<template>
  <section class="about">
    <CloseButton></CloseButton>
    <article>
      <h2>about</h2>
      <div class="about-text">
        <p>2013年 都内某4年制大学経済学部に入学</p>
        <p>2016年 専門商社の営業職に新卒入社。</p>
        <p>2017年 退職。</p>
        <p>2017年 訓練校にてプログラミング学習(Java)。</p>
        <p>2018年 SIerに入社しSEに転職。</p>
      </div>
    </article>
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
.about {
  background-color: rgba(157, 177, 202, 0.37);
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  position: fixed;
  margin: auto;
  width: 75%;
  height: 70%;
  border-radius: 50%;
  article {
    padding: 4% 12%;
    color: rgb(172, 164, 164);
    h2 {
      font-size: 2.8vw;
      text-decoration: underline;
      letter-spacing: 1.8vw;
    }
    .about-text {
      margin: 3% 7% 0;
      p {
        letter-spacing: 0.6vw;
        font-size: 1.4vw;
        margin: 3rem 0;
      }
    }
  }
}
@media (max-width: 767px) {
  .about {
    width: 160%;
    transform: translateX(-19%);
    article {
      padding: 7vh 0 5% 21%;
      h2 {
        font-size: 6.5vw;
        letter-spacing: 2.3vw;
      }
      .about-text {
        margin: 10% 5% 0;
        p {
          letter-spacing: 0.4vw;
          font-size: 3.5vw;
          margin: 1.5rem 0;
        }
      }
    }
  }
}
</style>
