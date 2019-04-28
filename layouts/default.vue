<template>
  <body>
    <BackgroundBar></BackgroundBar>
    <nuxt />
    <LinkArea></LinkArea>
  </body>
</template>

<script>
import BackgroundBar from '~/components/BackgroundBar.vue'
import LinkArea from '~/components/LinkArea.vue'

export default {
  components: {
    BackgroundBar,
    LinkArea
  }
}
</script>

<style scoped lang="scss"></style>
