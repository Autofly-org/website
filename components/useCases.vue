<template>
  <div class="container">
    <h2>Use Cases</h2>

    <div class="useCase left">
      <div class="img">
        <img src="/images/agriculture.jpg" />
        <p>We are using machine learning to analyze forsests and fields</p>
      </div>
      <div class="card">
        <h3>Agriculture &amp; Forest analysis</h3>
      </div>
    </div>

    <div class="useCase right">
      <div class="img">
        <img src="/images/rescue.jpg" />
        <p>Transporting Medical supplys or searching for drowning people</p>
      </div>
      <div class="card">
        <h3>Rescue &amp; Transport</h3>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container {
  .useCase {
    margin: 30px;
    position: relative;

    .img {
      position: relative;

      img {
        max-width: 70%;
        max-height: 70vh;
        border-radius: 30px;
      }

      p {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        display: inline-block;
      }
    }

    .card {
      background: #fff;
      border-radius: 30px;
      padding: 30px;
      display: inline-block;
      position: absolute;
      top: 50px;
      left: 60%;

      h3 {
        color: #000;
      }
    }
  }

  .right {
    p {
      width: 300px;
    }
  }
}
</style>
