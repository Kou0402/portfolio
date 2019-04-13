<template>
  <body>
    <nuxt />
  </body>
</template>

<script>
export default {
  mounted() {
    // ビューポートの高さを取得し、0.01を掛けて1%の値を算出して、vh単位の値を取得
    const vh = window.innerHeight * 0.01
    // カスタム変数--vhの値をドキュメントのルートに設定
    document.documentElement.style.setProperty('--vh', `${vh}px`)
  }
}
</script>
