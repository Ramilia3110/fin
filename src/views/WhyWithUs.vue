<template>
  <div id="why-with-us">
    <h1>Why you should learn with us?</h1>
    <div class="box-container">
      <div class="box1">
        <h4>PRACTICAL</h4>
        <p>
          The simulations are the results of R&D in which various corporate
          finance, leveraged finance and risk professionals contributed. From
          finance foundations to complex corporate valuations, the realistic
          practical application is in every stage.
        </p>
      </div>
      <div class="box2">
        <h4>ENGAGING</h4>
        <p>
          The simulations involve competition between teams and risk-taking
          elements to excite people. The energy throughout the process is
          intense given the competitive elements while analysing, discussing,
          pitching and negotiating financial instruments and companies.
        </p>
      </div>
      <div class="box3">
        <h4>INNOVATIVE</h4>
        <p>
          We offer a highly innovative training concept immersing participants
          in various investment banking tasks and leveraging stochastic
          modelling techniques to gamify the learning at the right pace.
        </p>
      </div>
      <div class="box4">
        <h4>PARTICIPANTS ARE LOVING IT</h4>
        <p>
          Teams run their simulated investment bank and watch their own P&L rise
          and fall. They compete against each other in their own market, not
          against a computer. The gamification of learning technical corporate
          finance skills leads to very high participant satisfaction.
        </p>
      </div>
      <div class="box5">
        <h4>ONGOING SUPPORT</h4>
        <p>
          We support clients beyond a particular training event. Our products
          are tailored towards clients’ needs and follow up consultations as
          well as testing options are available.
        </p>
      </div>
      <div class="box6">
        <h4>VALUE FOR MONEY</h4>
        <p>
          Our products are cost-effective because participants learn practical
          skills in a short time-frame, and they can directly apply what they
          have learned. Participants returning to their desk have a better
          understanding of their tasks and have gained a big picture
          understanding of different departments.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WhyWithUs"
};
</script>

<style lang="scss" scoped>
#why-with-us {
  padding-top: 7rem;
}
h1 {
  font-size: 4.5rem;
  font-weight: 500;
  color: #061b2e;
}
.box-container {
  margin: 9rem 0 5rem 0;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(30rem, 1fr));
  grid-gap: 6rem;
  align-items: start;
  h4 {
    font-size: 2.1rem;
    font-weight: 200;
  }
  p {
    margin-top: 2rem;
    text-align: justify;
    font-size: 1.8rem;
    line-height: 2.8rem;
  }
}
@media only screen and (max-width: 992px) {
  p {
    font-size: 1.6rem;
  }
}
@media only screen and (max-width: 768px) {
  .box-container {
    margin: 5rem 0 5rem 0;
    h4 {
      font-size: 1.8rem;
    }
    p {
      font-size: 1.6rem;
    }
  }
  h1 {
    font-size: 3rem;
  }
}
</style>
