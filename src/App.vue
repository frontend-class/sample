<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">전화번호부</router-link>
      <router-link to="/simple">Simple</router-link>
      <router-link to="/move-to">Move To</router-link>
      <router-link to="/hello/default">Hello Name</router-link>
    </div>
    <div class="main">
      <router-view/>
    </div>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  display: flex;
  width: 100%;
  justify-content: space-around;
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
.main {
  display: flex;
}
</style>
