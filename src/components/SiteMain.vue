<script>
import BannerVue from "./BannerVue.vue";
import ProductList from "./ProductList.vue";
export default {
  name: "SiteMain",
  components: {
    BannerVue,
    ProductList,
  },
};
</script>

<template>
  <main>
    <div class="container">
      <ProductList />
    </div>
    <!-- /.container -->

    <BannerVue />
  </main>
</template>
