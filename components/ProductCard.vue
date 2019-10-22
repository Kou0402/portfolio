<template>
  <article class="product-card-container">
    <a :href="productUrl" class="product-title-link">
      {{ productName }}
    </a>
    <div class="product-description">
      <p v-for="item in productDescription" :key="item.id">{{ item }}</p>
    </div>
    <img :src="productImgPath" class="product-img" />
  </article>
</template>

<script>
export default {
  props: {
    productUrl: {
      type: String,
      default: ''
    },
    productName: {
      type: String,
      default: ''
    },
    productDescription: {
      type: Array,
      default: function() {
        return []
      }
    },
    productImg: {
      type: String,
      default: ''
    }
  },
  data() {
    return {
      productImgPath: require('~/assets/img/' + this.productImg)
    }
  }
}
</script>

<style lang="scss" scoped>
.product-card-container {
  margin-bottom: 4rem;
  display: grid;
  align-items: center;
  grid-template-rows: 40px 200px;
  grid-template-columns: 1fr 300px;
  .product-title-link {
    grid-row: 1;
    grid-column: 1;
    text-decoration: underline;
    letter-spacing: 0.4vw;
    margin: 3vh 0;
    font-size: 2.4rem;
    color: white;
  }
  .product-description {
    grid-row: 2;
    grid-column: 1;
    padding-right: 0.3rem;
    p {
      letter-spacing: 0.2rem;
      line-height: 1.7rem;
      font-size: 1.3rem;
      margin-top: 1.7rem;
    }
  }
  .product-img {
    width: 300px;
    grid-row: 2;
    grid-column: 2;
  }
}
</style>
