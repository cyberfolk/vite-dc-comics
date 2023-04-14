<script>
export default {
  name: "ProductItem",
  props: {
    src: String,
  },
};
</script>

<template>
  <div class="col">
    <div class="product">
      <img :src="src" />
    </div>
  </div>
</template>

<style scoped>
img {
  height: 180px;
  width: 100%;
  object-fit: cover;
}
</style>
