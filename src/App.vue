<template>
  <div id="app">
    <VueLogo />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import VueLogo from "./assets/logo.svg";

export default {
  name: "App",
  components: {
    HelloWorld,
    VueLogo
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

svg {
  width: 200px;
  transition: all 0.3s ease;
}

svg:hover {
  transform: scale(1.1);
}
</style>
