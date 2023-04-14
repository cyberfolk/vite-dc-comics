<script>
import banner from "../data/banner.js";
export default {
  name: "BannerVue",
  components: {},
  data() {
    return {
      banner: banner,
    };
  },

  methods: {
    getImageUrl(name) {
      return new URL(`../assets/img/${name}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <section class="banner">
    <div class="container">
      <nav class="nav d-flex justify-content-around">
        <a class="nav-link d-flex" href="#" v-for="item in banner">
          <img :src="getImageUrl(item.src)" alt="digital-comics" />
          <div class="align-self-center">{{ item.name }}</div>
        </a>
      </nav>
    </div>
    <!-- /.container -->
  </section>
  <!-- /.banner -->
</template>
