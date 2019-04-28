<template>
  <section class="link-area">
    <router-link to="/" class="link">About >></router-link>
    <router-link to="/" class="link">Project >></router-link>
    <router-link to="/" class="link">Product >></router-link>
  </section>
</template>

<style lang="scss" scoped>
.link-area {
  position: fixed;
  bottom: 11vh;
  display: inline-flex;
  width: 70%;
  justify-content: space-between;
  left: 50%;
  transform: translateX(-50%);
  .link {
    font-size: 3rem;
    text-decoration: none;
    color: white;
  }
}
</style>
