<template>
  <transition name="page-title" appear>
    <h1>
      <slot></slot>
    </h1>
  </transition>
</template>

<style lang="scss" scoped>
h1 {
  letter-spacing: 3vw;
  text-indent: 5vw;
  margin: 9vh auto;
  color: #ff8c00;
  background: linear-gradient(to right, #ff8132, #ff28ff 45%, #89fffd 75%);
  background-clip: text;
  -webkit-text-fill-color: transparent;
  display: inline-block;
  font-family: 'Slabo 27px', serif;
  position: fixed;
  left: 50%;
  transform: translateX(-50%);
}

/* transition */
.page-title-enter {
  opacity: 0;
  transform: translate(-50%, 3rem);
}
.page-title-enter-active {
  transition: opacity 1s, transform 1s;
}

@media screen and (max-width: 896px) {
  h1 {
    letter-spacing: 4.2vw;
    text-indent: 6.5vw;
    margin: 10vh auto;
  }
}
</style>
