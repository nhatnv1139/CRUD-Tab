<template>
  <div id="app">
    <nav>
      <router-link to="/" class="button back">Home</router-link> |
      <router-link to="/about"
        ><a class="button primary">&nbsp;New Post</a></router-link
      >
    </nav>
    <router-view></router-view>
  </div>
</template>
<style scope>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  box-sizing: border-box;
  /* font-family: 'Mingzat', sans-serif; */
}
nav {
  padding: 30px;
}
nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
}
nav a.router-link-exact-active {
  color: #42b983;
}
.button {
  font-family: "Open Sans"; 
  font-size: 24px;
  font-weight: 400;
  display: inline-block;
  color: #fff;
  border-radius: 0.25em;
}
.back {
  line-height: 35px;
  transition: ease-in-out 0.2s;
  padding: 0 10px;
  color: rgb(46, 204, 113);
}
.back:hover,
.condensed:hover,
.touch:hover {
  transform: scale(1.05);
  box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2),
    inset 0 0 0 99999px rgba(0, 0, 0, 0.2);
}
.primary {
  line-height: 35px;
  transition: ease-in-out 0.2s;
  padding: 0 10px;
  color: black;
}
.primary:hover,
.condensed:hover,
.touch:hover {
  transform: scale(1.02);
  box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2),
    inset 0 0 0 99999px rgba(0, 0, 0, 0.2);
}
.new {
  background: rgb(46, 204, 113);
}
.touch {
  transition: ease-in-out 0.2s;
  line-height: 40px;
  width: 40px;
  padding: 0px;
  text-align: center;
}
.edit {
  background: rgb(52, 152, 219);
}
.delete {
  background: rgb(192, 57, 43);
}
</style>
