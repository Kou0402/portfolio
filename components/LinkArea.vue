<template>
  <section class="link-area">
    <router-link to="/about" class="link">About >></router-link>
    <router-link to="/work" class="link">Work >></router-link>
    <router-link to="/product" class="link">Product >></router-link>
  </section>
</template>

<style lang="scss" scoped>
.link-area {
  position: fixed;
  bottom: 9vh;
  display: inline-flex;
  width: 70%;
  justify-content: space-between;
  left: 50%;
  transform: translateX(-50%);
  .link {
    font-size: 2.5vw;
    text-decoration: none;
    color: white;
    font-family: 'Slabo 27px', serif;
  }
}
@media screen and (max-width: 896px) {
  .link-area {
    bottom: 11vh;
    width: 85%;
    .link {
      font-size: 5vw;
    }
  }
}
</style>
