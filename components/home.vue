<template>
  <div class="container">
    <a href="https://github.com/johann-su/autonomous-airplane">
      <img src="/images/github.svg" alt="">
      <p>View the code on Github</p>
    </a>
    <img src="/images/plane.svg" class="background">
    <div class="center">
      <h1>Autofly</h1>
      <p>A plane to save lives and give new insights</p>
    </div>
    <div class="contributors">
      <a href="https://github.com/HannHank">HannHank</a>
      <a href="https://github.com/johann-su">johann-su</a>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component
export default class Home extends Vue {

}
</script>


<style lang="scss" scoped>
.container {
  height: calc(100vh - 100px);
  display: flex;
  flex-direction: column;

  a {
    display: flex;
    flex-direction: row;
    align-items: center;
    text-decoration: none;

    p {
      margin-left: 20px;
    }
  }

  .background {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 70%;
  }

  .center {
    z-index: 3;
    align-self: center;
    margin: auto 0;
  }

  .contributors {
    display: flex;
    flex-direction: row;
  }
}
</style>

