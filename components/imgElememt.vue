<template>
  <div class="useCase" :class="{right: right}">
    <div class="card">
      <h3>{{ title }}</h3>
    </div>
    <div class="img">
      <img :src="img">
      <p>{{ msg }}</p>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component, Prop } from 'nuxt-property-decorator'

@Component
export default class imgElememt extends Vue {
  @Prop(String) readonly title: String | undefined
  @Prop(String) readonly img: String | undefined
  @Prop(String) readonly msg: String | undefined
  @Prop(Boolean) readonly right: Boolean | undefined
}
</script>

<style lang="scss" scoped>
.useCase {
  position: relative;

  &.right {
    text-align: right;
  }

  .img {
    position: relative;
    width: 50%;
    display: inline-block;
    z-index: 1;

    img {
      width: 100%;
      border-radius: 30px;
      max-height: 500px;
      object-fit: cover;
    }

    p {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }

  .card {
    border-radius: 30px;
    background: #fff;
    padding: 15px 30px;
    display: inline-block;
    position: absolute;
    top: 30%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 2;

    h3 {
      color: #000;
      display: inline-block;
    }
  }
}

@media only screen and (min-width: 1200px) {
  .useCase {
    width: 800px;
    margin: 40px auto;
  }
}

@media only screen and (max-width: 765px) {
  .right, .useCase {
    text-align: center !important;
  }

  .card {
    position: static !important;
    top: 0 !important;
    left: 0 !important;
    transform: none !important;
    padding: 5px 10px !important;
    display: inline-block;
    width: 80%;
    text-align: center;
    margin: 10px auto;
  }

  .img {
    width: 100% !important;
  }
}
</style>
