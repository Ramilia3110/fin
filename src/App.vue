<template>
  <div id="app">
    <div id="nav">
      <div class="container-nav">
        <div class="logo">
          <h1>
            <a href="#">
              <span>Fin</span>simco
            </a>
          </h1>
        </div>

        <ul>
          <li>
            <a href="#">Home</a>
          </li>
          <li>
            <a href="#about">About</a>
          </li>
          <li>
            <a href="#why-with-us">Why Us</a>
          </li>
          <li>
            <a href="#how-it-works">How it works</a>
          </li>
          <li>
            <a href="#staff-cards">Team</a>
          </li>
          <li>
            <a href="#contact">Contact</a>
          </li>
        </ul>
      </div>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
$primary-color: #011930;
*,
*::before,
*::after {
  box-sizing: inherit;
  margin: 0;
  padding: 0;
}
html {
  font-size: 62.5%;
  scroll-behavior: smooth;
}
body {
  box-sizing: border-box;
  background-color: #fff;
  width: 100%;
  height: 100%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  width: 100%;
  background-color: $primary-color;
  position: fixed;

  z-index: 10;
}
.container-nav {
  width: 90%;
  margin: 0 auto;
  padding: 0.5rem 2rem;
  display: flex;
  justify-content: space-between;
  align-self: center;
}
.logo h1 a {
  font-size: 3.5rem;
  font-weight: bold;
}
a {
  color: #fff;
  text-decoration: none;
}
span {
  color: #2d6aa8;
}
#nav ul {
  height: 8vh;
  width: 50%;
  display: flex;

  padding: 0.8rem;
  font-weight: 300;
  justify-content: space-around;
  align-items: center;
  li {
    list-style: none;
    a {
      font-size: 2rem;
      padding: 1.2rem;

      &:hover {
        background: #2d6aa8;
      }
    }
  }
}
</style>
