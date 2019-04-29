<template>
  <main>
    <PageTitle>About</PageTitle>
    <ContentsArea>
      <article>
        <h2>Career</h2>
        <p>2013年 都内某4年制大学経済学部に入学</p>
        <p>2016年 専門商社の営業職に新卒入社。</p>
        <p>2017年 退職。</p>
        <p>2017年 訓練校にてプログラミング学習(Java)。</p>
        <p>2018年 SIerに入社しSEに転職。</p>
      </article>
      <article>
        <h2>Skill</h2>
        <p>2013年 都内某4年制大学経済学部に入学</p>
        <p>2016年 専門商社の営業職に新卒入社。</p>
        <p>2017年 退職。</p>
        <p>2017年 訓練校にてプログラミング学習(Java)。</p>
        <p>2018年 SIerに入社しSEに転職。</p>
      </article>
    </ContentsArea>
  </main>
</template>

<script>
import PageTitle from '~/components/PageTitle.vue'
import ContentsArea from '~/components/ContentsArea.vue'

export default {
  components: {
    PageTitle,
    ContentsArea
  }
}
</script>

<style scoped lang="scss">
h2 {
  text-decoration: underline;
  letter-spacing: 1vw;
  margin: 3vh 0;
}
p {
  letter-spacing: 0.5vw;
  line-height: 2em;
}
@media screen and (max-width: 896px) {
  p {
    letter-spacing: 0.1vw;
    line-height: 2em;
  }
}
</style>
