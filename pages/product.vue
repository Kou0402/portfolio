<template>
  <main>
    <PageTitle>Product</PageTitle>
    <ContentsArea>
      <ProductCard
        :product-url="helloWorld.productUrl"
        :product-name="helloWorld.productName"
        :product-description="helloWorld.productDescription"
        :product-img="helloWorld.productImg"
      ></ProductCard>
      <ProductCard
        :product-url="portfolioLibrary.productUrl"
        :product-name="portfolioLibrary.productName"
        :product-description="portfolioLibrary.productDescription"
        :product-img="portfolioLibrary.productImg"
      ></ProductCard>
    </ContentsArea>
  </main>
</template>

<script>
import PageTitle from '~/components/PageTitle.vue'
import ContentsArea from '~/components/ContentsArea.vue'
import ProductCard from '~/components/ProductCard.vue'

export default {
  components: {
    PageTitle,
    ContentsArea,
    ProductCard
  },
  data() {
    return {
      helloWorld: {
        productUrl: 'https://kou-bfly.netlify.com',
        productName: 'Hello world!',
        productDescription: [
          'ポートフォリオサイトです。『Hello,world!』',
          'はバンド『BUMP OF CHICKEN』の『Butterflies』',
          'というアルバムの収録曲です。',
          'サイトを作成する際に何かテーマを決めて作ろうと思い',
          '自分の好きなバンドのアルバムをテーマにしました。',
          '使用技術：Nuxt.js, Netlify'
        ],
        productImg: 'hello_world.png'
      },
      portfolioLibrary: {
        productUrl: 'https://portfolio-library.com',
        productName: 'Portfolio Library',
        productDescription: [
          'エンジニア・デザイナー向けのポートフォリオ共有',
          'サイト。ポートフォリオを作成しようと思った時に',
          '面白いポートフォリオサイトが沢山あることを知り',
          'それらが眠っているだけではもったいないと感じ',
          '共有できる場があればいいと思い作成しました。',
          '使用技術：Nuxt.js, Firebase'
        ],
        productImg: 'portfolio_library.png'
      }
    }
  }
}
</script>

<style scoped lang="scss"></style>
