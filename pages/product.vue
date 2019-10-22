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
          '自分の好きなバンドのアルバムをテーマにしました。'
        ],
        productImg: 'hello_world.png'
      }
    }
  }
}
</script>

<style scoped lang="scss"></style>
