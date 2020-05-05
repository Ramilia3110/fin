<template>
  <div class="intro">
    <div class="container">
      <div class="slider">
        <div class="slide slide1">
          <div class="caption">
            <h1>IB Bootcamp</h1>
            <h4>(virtual & in-classroom, 1-day to 10-days)</h4>
            <p>For: Students with none to basic corporate finance skills. Some might have gained prior internship experience</p>
            <p>Focus: Essential Excel skills, accounting, basic financial modelling and PPT</p>
          </div>
        </div>
        <div class="slide slide2">
          <div class="caption">
            <h1>Summer Intern Simulation</h1>
            <h4>(virtual & in-classroom, 1⁄2-day to 10-days)</h4>
            <p>For: 2nd & 3rd year students. Some might have interned and study a finance related field</p>
            <p>Focus: Overview of key IB services, valuation methods and basic financial modeling</p>
          </div>
        </div>
        <div class="slide slide3">
          <div class="caption">
            <h1>Analyst Simulation</h1>
            <h4>(virtual & in-classroom, 1⁄2-day to 10-days)</h4>
            <p>For: 1st and 2nd year graduates who have gained some corporate finance related work experience</p>
            <p>Focus: Valuation methods and financial modeling</p>
          </div>
        </div>
        <div class="slide slide4">
          <div class="caption">
            <h1>Student Assessment Simulation</h1>
            <h4>
              Data about students performance is provided to clients. Features
              assessed:
            </h4>
            <ul>
              <li>Teamwork & communication skills</li>
              <li>Analytical thinking & sound judgement skills</li>
              <li>
                Attitude in time precious situations & capability to focus on
                relevant tasks
              </li>
              <li>Improvements during repeated tasks</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.intro {
  margin: 3rem 0 15rem 0;
}
.container {
  position: relative;
  width: 100%;
  height: 80vh;
  background-image: url("./../assets/bg2.jpg");
  background-position: center 60%;
  background-size: cover;
  overflow: hidden;
  .slider {
    position: absolute;
    top: 0;
    left: 0;
    width: 500%;
    height: 100%;
    float: left;
    animation: move 8s linear infinite;
    animation-direction: alternate;
    animation-play-state: running;
  }
}
.container .slider .slide {
  position: relative;
  width: 20%;
  height: 100%;
  float: left;
  transition: 0.6s;
  .caption {
    position: absolute;
    bottom: 7%;
    left: 6rem;
    right: 6rem;
    height: 40vh;
    padding: 5rem;
    border-radius: 1rem;
    color: #fff;
    background: rgba($color: #2d6aa8, $alpha: 1);
    transition: 0.5s;
    h1 {
      margin: 0;
      padding: 0;

      font-size: 4rem;
      transition: 0.5s;
    }
    h4 {
      font-size: 2.2rem;
      margin-bottom: 2rem;
    }
    p,
    li {
      margin: 0;
      padding: 0;
      font-size: 1.9rem;
      transition: 0.5s;
    }
    ul {
      text-align: left;
      padding-left: 5rem;
    }
  }
}

@keyframes move {
  0% {
    left: 0;
  }
  25% {
    left: 0;
  }
  30% {
    left: -100%;
  }
  45% {
    left: -100%;
  }
  50% {
    left: -200%;
  }
  75% {
    left: -200%;
  }
  80% {
    left: -300%;
  }
  100% {
    left: -300%;
  }
}

@media only screen and (max-width: 1200px) {
  .container .slider .slide .caption {
    left: 2rem;
    right: 2rem;
    padding: 2.2rem;
    height: 35vh;
    h1 {
      margin: 0 0 1rem;
      font-size: 3.2rem;
    }
  }
}

@media only screen and (max-width: 768px) {
  .container {
    height: 50vh;
  }
  .container .slider .slide .caption {
    margin: auto 2rem;
    padding: 2rem;
    height: 40vh;

    h1 {
      font-size: 2rem;
    }
    h4 {
      font-size: 1.5rem;
    }
    li,
    p {
      font-size: 1.4rem;
    }
    ul {
      padding-left: 3rem;
    }
  }
}
</style>
