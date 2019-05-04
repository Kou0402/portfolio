<template>
  <div class="background-bar">
    <div class="bar1"></div>
    <div class="bar2"></div>
    <div class="bar3"></div>
    <div class="bar4"></div>
  </div>
</template>

<style lang="scss" scoped>
.background-bar {
  position: relative;
  opacity: 0.09;
  div {
    position: fixed;
    background-color: rgb(206, 206, 206);
    width: 930px;
    height: 11px;
    border-radius: 10px;
  }
  .bar1 {
    top: calc(50% - 255px);
    right: calc(50% - 130px);
    transform: rotate(30deg);
  }
  .bar2 {
    bottom: calc(50% - 218px);
    right: calc(50% - 130px);
    transform: rotate(-30deg);
  }
  .bar3 {
    top: calc(50% - 230px);
    left: calc(50% - 130px);
    transform: rotate(-30deg);
  }
  .bar4 {
    bottom: calc(50% - 242px);
    left: calc(50% - 130px);
    transform: rotate(30deg);
  }
}
@media screen and (max-width: 896px) {
  .background-bar {
    div {
      height: 9px;
    }
  }
}
</style>
