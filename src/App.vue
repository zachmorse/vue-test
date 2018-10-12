<template>
  <div id="app">
    <img class="coverShot" src="./assets/Cover.jpg">
    <HelloWorld msg="Kate Bowen"/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "app",
  components: {
    HelloWorld
  }
};
</script>

<style>
html {
  background-color: black;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* color: #2c3e50; */
  /* margin-top: 60px; */
}

.coverShot {
  width: 100vw;
  animation: 2s ease-in-out photoAnimation;
}

@keyframes photoAnimation {
  from {
    filter: opacity(0%);
  }
  to {
    filter: opacity(100%);
  }
}
</style>
