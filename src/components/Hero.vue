<template>
  <img :src="require(`@/assets/img/${pictureSrc}`)" :alt="alt" />
</template>

<script>
export default {
  name: "Hero",
  props: {
    pictureSrc: String,
    alt: String,
  },
};
</script>

<style>
</style>