<script>
export default {
  name: "SiteHeader",
  components: {},
  data() {
    return {
      pages: [
        {
          name: "CHARACTERS",
          href: "#",
        },
        {
          name: "COMICS",
          href: "#",
        },
        {
          name: "MOVIES",
          href: "#",
        },
        {
          name: "TV",
          href: "#",
        },
        {
          name: "GAMES",
          href: "#",
        },
        {
          name: "COLLECTIBLES",
          href: "#",
        },
        {
          name: "GAMES",
          href: "#",
        },
        {
          name: "VIDEOS",
          href: "#",
        },
        {
          name: "FANS",
          href: "#",
        },
        {
          name: "NEWS",
          href: "#",
        },
        {
          name: "SHOP",
          href: "#",
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
  <header class="mt-4 bg-white">
    <nav class="navbar navbar-expand-md navbar-light bg-light py-0">
      <div class="container">
        <a class="navbar-brand" href="#">
          <img height="80" src="./../assets/img/dc-logo.png" alt="dc-logo" />
        </a>
        <!-- /.navbar-brand -->
        <button class="navbar-toggler d-lg-none" type="button" data-bs-toggle="collapse" data-bs-target="#main_nav" aria-controls="#main_nav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <!-- /.navbar-toggler -->
        <div class="collapse navbar-collapse" id="main_nav">
          <ul class="navbar-nav ms-auto mt-2 mt-lg-0">
            <li class="nav-item" v-for="page in pages">
              <a class="nav-link" :href="page.href">{{ page.name }}</a>
            </li>
          </ul>
        </div>
        <!-- /#main_nav -->
      </div>
      <!-- /.container -->
    </nav>
    <!-- /.navbar -->
  </header>
</template>
