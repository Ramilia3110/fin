<template>
  <div id="how-it-works">
    <div class="container">
      <h1>How It Works?</h1>
      <div class="img-box">
        <img src="@/assets/Doughnut.svg" alt />
      </div>
      <ul>
        <li>Each simulation consists of 5 to 20 teams, with 2 to 4 members in each team.</li>
        <li>Each team is running its own Investment Bank with its own P&L.</li>
        <li>Teams compete against other teams in their own market, not against a computer. The decisions of each team influences the other teams’ results and the market development overall.</li>
        <li>
          Each team runs 4 departments:
          <ul>
            <li>M&A advisory</li>
            <li>Debt capital markets</li>
            <li>Equity capital markets</li>
            <li>Financial Sponsors Group</li>
          </ul>
        </li>
        <li>The simulation is run over 3 to 6 rounds.New industry and company specific data is released in each round.</li>
        <li>After the introduction, the teams familiarise themselves with the decision making process, which in each round is influenced by the results of earlier rounds.</li>
      </ul>
      <div class="video-wrapper">
        <video autoplay muted id="bgVideo" controls>
          <source src="@/assets/2.mp4" type="video/mp4" />
        </video>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HowItWorks",
  data() {
    return {};
  }
};
</script>

<style lang="scss" scoped>
#how-it-works {
  padding: 15rem 1rem;
}
.container {
  margin: 3rem 0;
}
h1 {
  font-size: 4.2rem;
  font-weight: 500;
  color: #061b2e;
  margin-bottom: 7rem;
}
.img-box {
  width: 42rem;
  height: 42rem;
  border-radius: 50%;
  float: right;
  shape-outside: circle();
  margin: 0 1rem 1rem 2rem;
  img {
    margin-left: 3rem;
    width: 100%;
    height: 100%;
  }
}

ul {
  padding: 0 7rem 0 1rem;
  text-align: left;
  li {
    font-size: 2rem;
    line-height: 3.5rem;
  }
}
.video-wrapper {
  position: relative;
  margin: 2rem auto;
  min-width: 30rem;

  video {
    object-fit: cover;
  }
}

@media only screen and (max-width: 768px) {
  .how-it-works {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .img-box {
    width: 35rem;
    height: 35rem;
    float: none;
    margin: 0 auto;
    img {
      margin: 0 auto;
    }
  }
  ul {
    text-align: justify;
  }
}
@media only screen and (max-width: 992px) {
  ul {
    padding: 0 2rem 0 2rem;
    text-align: left;
    li {
      font-size: 1.6rem;
      line-height: 3rem;
    }
  }
}
.video-wrapper {
  margin-top: 5rem;
  width: 100%;
  min-width: 35rem;
  overflow: hidden;

  video {
    width: 100%;
    height: 100%;
    padding: 0 1rem;
  }
}
@media only screen and (max-width: 768px) {
  h1 {
    font-size: 3rem;
  }
}
</style>
