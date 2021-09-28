<template>
  <img :src="src" :alt="alt" />
</template>

<script>
export default {
  name: "Hero",
  props: {
    src: String,
    alt: String,
  },
};
</script>

<style>
</style>