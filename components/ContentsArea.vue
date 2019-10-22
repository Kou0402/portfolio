<template>
  <div class="background">
    <CloseButton></CloseButton>
    <transition name="content" appear>
      <section class="content">
        <slot></slot>
      </section>
    </transition>
  </div>
</template>

<script>
import CloseButton from '~/components/CloseButton.vue'

export default {
  components: {
    CloseButton
  }
}
</script>

<style lang="scss" scoped>
.background {
  background-color: rgba(195, 195, 195, 0.05);
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  position: fixed;
  margin: auto;
  width: 60%;
  height: 55%;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  .content {
    color: white;
    text-align: left;
    height: 90%;
    width: 80%;
    overflow-y: scroll;
  }
}

/* transition */
.content-enter {
  opacity: 0;
}
.content-enter-active {
  transition: opacity 2s;
}

@media screen and (max-width: 896px) {
  .background {
    width: 85%;
    .content {
      width: 90%;
    }
  }
}
</style>
