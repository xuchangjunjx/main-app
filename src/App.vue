<template>
  <div id="app-main-root">
    <div id="nav">
      <router-link to="/">main-app</router-link> |
      <router-link to="/sub-app-entry">sub-app1</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="less">
#app-main-root {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
