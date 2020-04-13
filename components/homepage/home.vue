<template>
  <div class="home">
    <img src="/images/plane.svg" class="bg-plane">

    <div class="heading">
      <h1>Autonomous Plane Project</h1>
      <h2>A plane to save lives and give new insights</h2>
    </div>

    <div class="contributors">
      <a href="https://www.github.com/hannHank">HannHank</a>
      <a href="https://www.github.com/johann-su">johann-su</a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.home {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: calc(100vh - 200px);
  margin-bottom: 100px;

  .bg-plane {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 80vw;
    z-index: 1;
  }

  .heading {
    margin: auto auto;
    z-index: 2;
  }

  a {
    margin: 10px;
  }
}

@media only screen and (max-width: 765px) {
  .contributors {
    text-align: center;
  }
}
</style>


