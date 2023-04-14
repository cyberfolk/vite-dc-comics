<script>
export default {
  name: "BannerVue",
  components: {},
  data() {
    return {
      banner: [
        {
          name: "DIGITAL COMICS",
          src: "buy-comics-digital-comics.png",
        },
        {
          name: "DC MERCHANANDISE",
          src: "buy-comics-merchandise.png",
        },
        {
          name: "SUBSCRIPTION",
          src: "buy-comics-subscriptions.png",
        },
        {
          name: "COMIC SHOP LOCATOR",
          src: "buy-comics-shop-locator.png",
        },
        {
          name: "DC POWER VISA",
          src: "buy-dc-power-visa.svg",
        },
      ],
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
