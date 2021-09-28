<template>
  <div class="title">
    <h1>
      {{ msg }}
    </h1>
  </div>
</template>

<script>
export default {
  name: "Title",
  props: {
    msg: String,
  },
};
</script>

<style>
h1 {
  animation-name: fluo;
  animation-direction: alternate;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
  animation-duration: 2s;
  color: #41bd84;
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