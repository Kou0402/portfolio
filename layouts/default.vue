<template>
  <body>
    <div class="background-bar">
      <div class="bar1"></div>
      <div class="bar2"></div>
      <div class="bar3"></div>
      <div class="bar4"></div>
    </div>
    <nuxt />
  </body>
</template>

<style scoped lang="scss">
.background-bar {
  position: relative;
  div {
    position: fixed;
    background-color: rgba(206, 206, 206, 0.096);
    width: 930px;
    height: 13px;
    border-radius: 10px;
  }
  .bar1 {
    top: 150px;
    left: -80px;
    transform: rotate(30deg);
  }
  .bar2 {
    top: 610px;
    left: -80px;
    transform: rotate(-30deg);
  }
  .bar3 {
    top: 170px;
    left: 590px;
    transform: rotate(-30deg);
  }
  .bar4 {
    top: 630px;
    left: 590px;
    transform: rotate(30deg);
  }
}
</style>
