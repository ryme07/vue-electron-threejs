<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view />
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  background: #000;
  margin: 0;
  overflow: hidden; /* Hide scrollbars */
}
.active a {
  color: #000;
}
nav {
  padding: 10px;
  background: transparent;
  position: absolute;
  width: 100%;
  background: transparent;
  a {
    font-weight: bold;
    color: #fff;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
