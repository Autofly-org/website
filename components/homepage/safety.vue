<template>
  <div class="savety">
    <h2>Safety</h2>
    <p>We are designing the Aircraft with high security standards. All critical Parts are going to be redundant. If no safe landing is possible, the Plane is going to have a parachute, that deploys automaticaly, when the aircraft is decending beyond a critical vertical speed. The parachute can also be deployed from the control station if nessesary.</p>
    <img src="/images/safety.svg">
  </div>
</template>

<style lang="scss" scoped>
.savety {
  text-align: center;
  margin-top: 40px;

  img {
    width: 40%;
  }
}

@media only screen and (min-width: 1200px) {
  p {
    width: 800px;
    margin: 0 auto;
  }
}

@media only screen and (min-width: 1200px) {
  img {
    width: 300px !important;
  }
}
</style>
