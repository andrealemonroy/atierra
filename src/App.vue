<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style>
.home {
  background: url("./assets/background-stars.png") no-repeat;
  width: 100vw;
  height: 100vh;
  background-size: cover;
  -o-background-size: cover;
  -moz-background-size: cover;
  -webkit-background-size: cover;
  color: #fff;
}

.home #nav a {
  color: #fff;
}

.home .typed {
  color: #fff !important;
}

#nav {
  padding: 20px;
  display: flex;
  justify-content: space-around;
  margin: auto 20%;
  color: #fff;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

.align-left {
  text-align: left;
}

.flex-around {
  display: flex;
  justify-content: space-around;
}

h1 {
  font-size: 42px !important;
}

.maxw-100 {
  max-width: 100%;
}

.maxw-50 {
  max-width: 50%;
}

.m-auto {
  margin: auto;
}

.font-22 {
  font-size: 22px;
}

.font-20 {
  font-size: 20px;
}

.align-center {
  text-align: center;
}

.br-50 {
  border-radius: 50%;
}
</style>
