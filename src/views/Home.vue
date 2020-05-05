<template>
  <div class="home">
    <Header />
    <div class="container">
      <About />
      <intro />
      <WhyWithUs />
      <Banner2 />
      <HowItWorks />
    </div>

    <div class="container">
      <StaffCards />
    </div>
    <Banner />
    <div class="container">
      <Contact />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import Header from "@/components/Header.vue";
import About from "./About.vue";
import WhyWithUs from "./WhyWithUs.vue";
import HowItWorks from "./HowItWorks.vue";
import StaffCards from "./StaffCards";
import Contact from "./Contact.vue";
import Banner from "@/components/Banner.vue";
import Banner2 from "@/components/Banner2.vue";
import Intro from "./Intro.vue";

export default {
  name: "Home",
  components: {
    About,
    Contact,
    Header,
    HowItWorks,
    WhyWithUs,
    StaffCards,
    Banner,
    Banner2,
    Intro
  }
};
</script>

<style lang="scss" scoped>
.container {
  width: 80%;
  margin: 3rem auto;
  padding: 3.5rem;
}
</style>
