<script>
export default {
  props: {
    thumb: String,
    series: String,
  },
};
</script>

<template>
  <div class="img-container">
    <img :src="thumb" alt="" />
  </div>

  <p>{{ series }}</p>
</template>

<style lang="scss" scoped>
img {
  width: 100%;
  height: 200px;
  object-fit: cover;

  object-position: 0 0;
}

.img-container {
  width: 200px;
  height: 200px;
  aspect-ratio: 1;
}
</style>
