<template>
  <h1>
    <slot></slot>
  </h1>
</template>

<style lang="scss" scoped>
h1 {
  letter-spacing: 5vw;
  text-indent: 5vw;
  margin: 12vh auto;
  color: #ff8c00;
  background: linear-gradient(to right, #ff8132, #ff28ff 45%, #89fffd 75%);
  background-clip: text;
  -webkit-text-fill-color: transparent;
  display: inline-block;
}
@media screen and (max-width: 896px) {
  h1 {
    letter-spacing: 6.5vw;
    text-indent: 6.5vw;
  }
}
</style>
