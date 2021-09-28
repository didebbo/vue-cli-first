<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <Title msg="La mia prima app con Vue CLI!" />
  </div>
</template>

<script>
import Title from "./components/Title.vue";

export default {
  name: "App",
  components: {
    Title,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

img {
  animation-name: fluo;
  animation-direction: alternate;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
  animation-duration: 2s;
}

@keyframes fluo {
  0% {
    filter: hue-rotate(0deg);
  }
  100% {
    filter: hue-rotate(360deg);
  }
}
</style>
