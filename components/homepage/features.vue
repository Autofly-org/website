<template>
  <div class="features">
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
      <h3>Safety</h3>
      <p>Safety for all types of missions</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.features {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: .5fr 1fr 1fr;
  margin-top: 40px;

  h2 {
    grid-column: 1 / span 2;
  }
}

@media only screen and (min-width: 1200px) {
  .features {
    width: 800px;
    margin: 40px auto;
  }
}

@media only screen and (max-width: 765px) {
  .features {
    grid-template-columns: 1fr 0fr;

    h2 {
      grid-column: 1;
    }

    .feature {
      grid-column: 1;
    }
  }
}
</style>
