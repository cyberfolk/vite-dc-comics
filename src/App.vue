<script>
export default {
  data() {
    return {
      msg: "SPERIAMO FUNZIONI",
    };
  },
};
</script>

<template>
  <header class="mt-4 bg-white">
    <div class="container">
      <div class="row">
        <div class="col-4 py-3 d-flex">
          <img class="align-self-center" src="./assets/img/dc-logo.png" alt="dc-log" />
        </div>
        <!-- /.col -->
        <div class="col-8 d-flex">
          <nav class="nav align-self-center">
            <a class="nav-link" href="#" aria-current="page">CHARACTERS</a>
            <a class="nav-link" href="#">COMICS</a>
            <a class="nav-link" href="#">MOVIES</a>
            <a class="nav-link" href="#">TV</a>
            <a class="nav-link" href="#">GAMES</a>
            <a class="nav-link" href="#">COLLECTIBLES</a>
            <a class="nav-link" href="#">VIDEOS</a>
            <a class="nav-link active" href="#">FANS</a>
            <a class="nav-link" href="#">NEWS</a>
            <a class="nav-link" href="#">SHOP</a>
          </nav>
        </div>
        <!-- /.col -->
      </div>
      <!-- /.row -->
    </div>
    <!-- /.container -->
  </header>

  <main>
    <section class="content"></section>
    <section class="banner"></section>
  </main>

  <footer>
    <div class="footer_up">
      <div class="container">
        <div class="row">
          <div class="col-6"></div>
          <!-- /.col-6 -->
          <div class="col-6">
            <img src="./assets/img/dc-logo-bg.png" alt="" />
          </div>
          <!-- /.col-6 -->
        </div>
        <!-- /.row -->
      </div>
      <!-- /.container -->
    </div>
    <!-- /.footer_up -->
    <div class="footer_down mb-4">
      <div class="container">
        <div class="row">
          <div class="col-6"></div>
          <!-- /.col-6 -->
          <div class="col-6"></div>
          <!-- /.col-6 -->
        </div>
        <!-- /.row -->
      </div>
      <!-- /.container -->
    </div>
    <!-- /.footer_down -->
  </footer>
</template>

<style lang="scss">
@use "./assets/scss/partials/variables" as *;
header {
  a {
    font-family: "Bahnschrift SemiBold";
    font-size: 0.9rem !important;
    color: $dark !important;
    position: relative;
  }

  .active {
    color: $accenture !important;
  }

  .active:after {
    content: "";
    position: absolute;
    right: 0;
    bottom: -100%;
    height: 6px;
    width: 100%;
    background-color: $accenture;
  }

  img {
    height: 80px;
  }
}

main {
  section {
    height: 100px;
  }

  .content {
    background-color: $dark;
  }

  .banner {
    background-color: $accenture;
  }
}

footer {
  .footer_up {
    background-image: url("./assets/img/footer-bg.jpg");
    background-size: cover;
    height: 500px;
  }

  .footer_down {
    background-color: $darkless;
    height: 100px;
    position: relative;
    z-index: 1;
  }
}
</style>
