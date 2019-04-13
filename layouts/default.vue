<template>
  <body id="body">
    <nuxt />
  </body>
</template>

<script>
export default {
  mounted() {
    function imageJustSize() {
      const bodyElement = document.getElementById('body')
      const windowHeight = window.innerHeight
      bodyElement.style.height = windowHeight + 'px'
    }

    imageJustSize()

    window.addEventListener('resize', imageJustSize)
  }
}
</script>
