<template>
  <div class="banner">
    <div class="clouds">
      <img class="cloud c1" src="@/assets/clouds/cloud1.png" style="--i:1;" alt="clouds" />
      <img class="cloud c2" src="@/assets/clouds/cloud2.png" style="--i:9;" alt="clouds" />

      <img class="cloud c3" src="@/assets/clouds/cloud3.png" style="--i:18;" alt="clouds" />

      <img class="cloud c4" src="@/assets/clouds/cloud4.png" style="--i:26;" alt="clouds" />
      <img class="cloud c5" src="@/assets/clouds/cloud5.png" style="--i:34;" alt="clouds" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Banner"
};
</script>

<style scoped lang="scss">
.banner {
  width: 100vw;
  height: 80vh;
  background-image: url("./../assets/cloud2.jpg");
  background-size: cover;
  background-position: 90% 70%;
  position: relative;
  margin: 15rem 0;
  border-radius: 0.5rem 0.5rem 0.8rem 0.8rem;
}
.clouds {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
  .cloud {
    position: absolute;
    bottom: 0;
    max-width: 100%;
    animation: animate ease-in-out infinite;
    animation-duration: 15s;
  }
  .c1 {
    animation-delay: 0;
  }
  .c2 {
    animation-delay: 1s;
  }
  .c3 {
    animation-delay: 3s;
  }
  .c4 {
    animation-delay: 5s;
  }
  .c5 {
    animation-delay: 7s;
  }
}

@keyframes animate {
  0% {
    transform: translateX(-100%);
    opacity: 0;
  }
  30% {
    opacity: 1;
  }
  100% {
    transform: translateX(100%);
  }
}
</style>