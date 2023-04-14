<script>
export default {
  name: "ProductItem",
  props: {
    src: String,
    title: String,
  },
  //Don't use method getImageUrl because the images is hosted on internet
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
