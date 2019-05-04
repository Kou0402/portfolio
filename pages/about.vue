<template>
  <main>
    <PageTitle>About</PageTitle>
    <ContentsArea>
      <article>
        <h2>Career</h2>
        <p>2013年 成城大学経済学部に入学。</p>
        <p>2016年 営業職として専門商社に入社。</p>
        <p>2017年 退職。</p>
        <p>2017年 職練校にてWebプログラミング講座受講。</p>
        <p>2018年 SEとしてSIerに転職。</p>
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
      <article>
        <h2>SNS</h2>
        <div class="sns-link-area">
          <a href="https://twitter.com/ko_u_0402?lang=ja" class="sns-link">
            <img class="sns-image" src="~/assets/img/twitter.svg" />
          </a>
          <a href="https://qiita.com/ko_u_0402" class="sns-link">
            <img class="sns-image" src="~/assets/img/qiita.png" />
          </a>
          <a href="https://github.com/Kou0402" class="sns-link">
            <img class="sns-image github-image" src="~/assets/img/github.svg" />
          </a>
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
  font-family: 'Slabo 27px', serif;
}
p {
  letter-spacing: 0.3vw;
  line-height: 1.5em;
}
.skillcard-area {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.sns-link-area {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  .sns-link {
    width: 16rem;
    margin: 0 1.4vw 2.5vh;
    text-align: center;
    .sns-image {
      width: auto;
      height: 7rem;
    }
    .github-image {
      background-color: white;
    }
  }
}
@media screen and (max-width: 896px) {
  p {
    letter-spacing: 0;
    line-height: 1.3em;
  }
  .sns-link-area {
    .sns-link {
      width: 8rem;
      margin: 0 1.8vw 2vh;
      .sns-image {
        height: 4rem;
      }
    }
  }
}
</style>
