<template>
  <div class="about" id="about">
    <h1>About Us</h1>
    <div class="about-us__container">
      <div class="about-box">
        <div class="box1">
          <p>
            Finsimco is pioneering in investment banking simulations. Our
            simulations are the most challenging and realistic available for
            training corporate finance professionals.We provide experiential learning
            in an exciting, virtual business environment.
            The combination of immediate feedback and the competitive group
            dynamics are unbeatable for consolidating learning and acquiring skills.
          </p>
        </div>
        <div class="box2">
          <p>Our modular-based investment banking simulations are:</p>
          <ul class="list">
            <li>
              tailored to
              the target audience - intern, analyst and associate levels,
            </li>
            <li>available as a 1/2-day to 10-day product,</li>
            <li>
              flexible to allow the inclusion of further
              corporate finance fields besides the core M&A and Capital Markets
              modules.
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.about {
  transition: all 500ms ease-in;
}
h1 {
  padding: 15rem 0 7rem 0;
  color: #061b2e;
  font-size: 4.2rem;
  font-weight: 500;
}
.about-us__container {
  margin-bottom: 12rem;
}

.about-box {
  display: grid;
  grid-auto-columns: 1fr 1fr;
  grid-template-areas: "box1 box2";
}
.box1 {
  grid-area: box1;
  p::first-letter {
    color: #1e4975;
    font-weight: 300;
    font-size: 2.5rem;
  }
}
.box2 {
  grid-area: box2;
  margin-left: 8rem;
}

p,
li {
  text-align: justify;
  font-size: 2rem;
  font-weight: 200;
  line-height: 4.1rem;
}

.list {
  margin-left: 2.3rem;
}

@media only screen and (max-width: 992px) {
  .about-box {
    display: flex;
    flex-direction: column;
  }

  .box2 {
    margin-left: 0;
  }
  .list {
    margin-left: 5rem;
  }
}
</style>
