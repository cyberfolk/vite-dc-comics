<script>
export default {
  name: "ProductItem",
  props: {
    src: String,
    title: String,
  },
};
</script>

<template>
  <div class="col">
    <div class="product">
      <img :src="src" />
      <div class="title">{{ title }}</div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables" as *;
img {
  height: 180px;
  width: 100%;
  object-fit: cover;
}

.title {
  text-transform: uppercase;
  color: $light;
  font-size: 0.8rem;
}
</style>
