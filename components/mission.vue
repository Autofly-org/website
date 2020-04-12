<template>
  <div class="container">
      <h2>The Mission</h2>
      <p>We want to build a autonomous plane that can execute missions autonomously.  Usecases include analyzing agicultural land, forest health or rescueing people.</p>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component
export default class Mission extends Vue {

}
</script>


<style lang="scss" scoped>
.container {
  background: #fff;
  border-radius: 30px;
  padding: 30px;
  max-width: 1200px;
  display: inline-block;

  h2, p {
    color: #000;
  }

  h2 {
    margin-bottom: 20px;
  }
}
</style>
