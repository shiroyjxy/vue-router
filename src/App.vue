<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/text">Text</router-link>
    </div>
    <router-view/>
    <div class="footer">
      <h2>footer内容</h2>
    </div>
  </div>
</template>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  background-color: aqua;
  padding: 30px;
  a {
    font-weight: bold;
    font-size: 30px;
    margin-left: 50px;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
      background-color: yellow;
    }
  }
}
.footer{
  height: 200px;
  background-color: #2c3e50;
  h2{
    font-size: 20px;
    color: antiquewhite;
  }
}
</style>
