<template>
  <div>
    <div class="center">
      <h1>404</h1>
      <nuxt-link to="/">Go Home</nuxt-link>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.center {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;

    h1 {
      font-size: 60px;
    }
}
</style>