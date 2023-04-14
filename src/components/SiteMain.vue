<script>
import BannerVue from "./BannerVue.vue";
import ProductList from "./ProductList.vue";
import JumbotronVue from "./JumbotronVue.vue";
export default {
  name: "SiteMain",
  components: {
    BannerVue,
    ProductList,
    JumbotronVue,
  },
};
</script>

<template>
  <main>
    <JumbotronVue />
    <ProductList />
    <BannerVue />
  </main>
</template>
