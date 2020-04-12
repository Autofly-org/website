<template>
  <div class="container">
    <h2>Features</h2>
    <div class="feature">
      <h3>VTOL</h3>
      <p>Enables the Aircraft to access difficult places</p>
    </div>
    <div class="feature">
      <h3>Autonomous</h3>
      <p>For large scale operations without human supervision</p>
    </div>
    <div class="feature">
      <h3>Long Range</h3>
      <p>1 hour flight time for long missions</p>
    </div>
    <div class="feature">
      <h3>Safe</h3>
      <p>Safety for all types of missions</p>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component
export default class Features extends Vue {

}
</script>


<style lang="scss" scoped>
.container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(3, 1fr);
  gap: 25px;

  h2 {
    grid-column: 1 / span 2;
  }

  .feature {
    &:nth-of-type(odd) {
      grid-column: 1;
    }
    &:nth-of-type(even) {
      grid-column: 2;
    }

    h3 {
      margin-bottom: 10px;
    }
  }
}
</style>
