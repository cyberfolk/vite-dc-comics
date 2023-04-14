<script>
import BannerVue from "./BannerVue.vue";
export default {
  name: "SiteMain",
  components: {
    BannerVue,
  },
};
</script>

<template>
  <main>
    <section class="content">
      <div class="container"></div>
      <!-- /.container -->
    </section>
    <!-- /.content -->

    <BannerVue />
  </main>
</template>
