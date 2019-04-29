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
        <div class="skillcard-area">
          <SkillCard file-name="java.svg" star="★★★☆☆"></SkillCard>
          <SkillCard file-name="php.svg" star="★★☆☆☆"></SkillCard>
          <SkillCard file-name="JavaScript.svg" star="★★★★☆"></SkillCard>
          <SkillCard file-name="spring.svg" star="★★★☆☆"></SkillCard>
          <SkillCard file-name="jquery.svg" star="★★★★☆"></SkillCard>
          <SkillCard file-name="vue.svg" star="★★★☆☆"></SkillCard>
        </div>
      </article>
    </ContentsArea>
  </main>
</template>

<script>
import PageTitle from '~/components/PageTitle.vue'
import ContentsArea from '~/components/ContentsArea.vue'
import SkillCard from '~/components/SkillCard.vue'

export default {
  components: {
    PageTitle,
    ContentsArea,
    SkillCard
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
  letter-spacing: 0.4vw;
  line-height: 2em;
}
.skillcard-area {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
@media screen and (max-width: 896px) {
  p {
    letter-spacing: 0;
    line-height: 2em;
  }
}
</style>
