<template>
  <div class="header">
    <div class="container"></div>
    <div class="video-wrapper">
      <video autoplay muted loop id="bgVideo">
        <source src="@/assets/hero.mp4" type="video/mp4" />
      </video>
      <div class="text-content">
        <h1>
          Want to be
          <span>among</span> experts?
        </h1>
        <p>Real-life financial simulations for junior investment bankers</p>
        <a href="#contact" class="btn">Contact Us</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style lang="scss" scoped>
.header {
  padding-top: 3rem;
  height: 100vh;
  border-bottom: solid 3px #1e4975;
  background-image: linear-gradient(
    rgba($color: #000000, $alpha: 0.5) 0%,
    rgba($color: #000000, $alpha: 0.6) 50%,
    rgba($color: #000000, $alpha: 0.3) 100%
  );
  color: rgba($color: #000000, $alpha: 1);
  margin-bottom: 3rem;
}
.video-wrapper {
  position: relative;
  width: 100%;
  height: 100%;
  overflow: hidden;
  video {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    min-width: 100%;
    min-height: 100%;
    width: 100vw;
    height: auto;
    z-index: -1;
    overflow: hidden;
    object-fit: cover;
  }
  .text-content {
    position: relative;
    top: 55%;
    transform: translateY(-50%);
    color: #fff;
    text-align: center;
    font-weight: bold;
    h1 {
      font-size: 7rem;
      margin-bottom: 1rem;
    }
    p {
      font-size: 4rem;
      padding: 0 25rem;
    }
    span {
      color: #2d6aa8;
    }
    .btn {
      display: inline-block;
      background: #011930;
      padding: 1.4rem 5rem;
      color: #fff;
      text-transform: uppercase;
      cursor: pointer;
      border-radius: 0.8rem;
      margin-top: 0.8rem;
      font-size: 1.4rem;
      &:hover {
        background: #357cc4;
        animation: animate 3s ease-in-out;
      }
    }
  }
}
@keyframes animate {
}
</style>
