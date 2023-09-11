<script>
export default {
  props: {
    thumb: String,
    series: String,
    price: String,
    type: String,
  },
};
</script>

<template>
  <div class="img-container">
    <img :src="thumb" alt="" />
    <div class="text-hover">
      <div class="central-text-hover">
        <p>Price: {{ price }}</p>
        <p>Type: {{ type }}</p>
      </div>
    </div>
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
  position: relative;
}
.text-hover {
  display: none;
  position: absolute;
  top: 0;
  bottom: 0;
  width: 200px;
  height: 200px;
  background-color: rgba(0, 0, 0, 0.6);
  .central-text-hover {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    text-align: center;
    justify-content: center;
  }
}
.img-container:hover .text-hover {
  display: block;
}
</style>
