<template>
  <div class="autofly-website">
    <head class="head">
      <nuxt-link to="/"><img src="/images/logo.svg" alt="Autofly logo" class="logo"></nuxt-link>
      <a href="https://www.github.com/autofly-org" class="github">
        <img src="/images/github.svg">
        <span>Visit us on Github</span>
      </a>
    </head>
    <nuxt />
  </div>
</template>

<style lang="scss">
.autofly-website {
  .head {
    margin: 50px 50px 0 50px;
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    justify-content: space-between;

    .github {
      display: inline-flex;
      flex-direction: row;
      justify-content: space-around;
      align-items: center;
      width: 250px;
    }

    .logo {
      width: 200px;
    }
  }
}

@media only screen and (max-width: 765px) {
  .head {
    flex-direction: column !important;

    .logo, .github {
      width: 40vw !important;
      margin: 20px 0;
    }
  }
}
</style>
