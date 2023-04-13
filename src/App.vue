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
    <section class="content">
      <div class="container"></div>
      <!-- /.container -->
    </section>
    <!-- /.content -->
    <section class="banner">
      <div class="container">
        <nav class="nav align-self-center">
          <a class="nav-link" href="#" aria-current="page">
            <img src="./assets/img/buy-comics-digital-comics.png" alt="" />
            <span>DIGITAL COMICS</span>
          </a>
          <a class="nav-link" href="#">
            <img src="./assets/img/buy-comics-merchandise.png" alt="" />
            <span>DC MERCHANANDISE</span>
          </a>
          <a class="nav-link" href="#">
            <img src="./assets/img/buy-comics-subscriptions.png" alt="" />
            <span>SUBSCRIPTION</span>
          </a>
          <a class="nav-link" href="#">
            <img src="./assets/img/buy-comics-shop-locator.png" alt="" />
            <span>COMIC SHOP LOCATOR</span>
          </a>
          <a class="nav-link" href="#">
            <img src="./assets/img/buy-dc-power-visa.svg" alt="" />
            <div>DC POWER VISA</div>
          </a>
        </nav>
      </div>
      <!-- /.container -->
    </section>
    <!-- /.banner -->
  </main>

  <footer>
    <div class="footer_up">
      <div class="container">
        <div class="row">
          <div class="col-6">
            <div class="row">
              <div class="col-3">
                <h2>DC COMICS</h2>
                <ul>
                  <li><a href="#">Characters</a></li>
                  <li><a href="#">Comics</a></li>
                  <li><a href="#">Movies</a></li>
                  <li><a href="#">TV</a></li>
                  <li><a href="#">Games</a></li>
                  <li><a href="#">Videos</a></li>
                  <li><a href="#">News</a></li>
                </ul>
                <h2>SHOP</h2>
                <ul>
                  <li><a href="#">Shop DC</a></li>
                  <li><a href="#">Shop DC Collectibles</a></li>
                </ul>
              </div>
              <!-- /.col-3 -->

              <div class="col-3">
                <h2>DC</h2>
                <ul>
                  <li><a href="#">Term Of Use</a></li>
                  <li><a href="#">Privacy polici (News)</a></li>
                  <li><a href="#">Ad Choices</a></li>
                  <li><a href="#">Advertising</a></li>
                  <li><a href="#">Jobs</a></li>
                  <li><a href="#">Subscriptions</a></li>
                  <li><a href="#">Talent Workshops</a></li>
                  <li><a href="#">CPSC Certificates</a></li>
                  <li><a href="#">Ratings</a></li>
                  <li><a href="#">Shop Help</a></li>
                  <li><a href="#">Contact Us</a></li>
                </ul>
              </div>
              <!-- /.col-3 -->

              <div class="col-3">
                <h2>SITES</h2>
                <ul>
                  <li><a href="#">DC</a></li>
                  <li><a href="#">MAD Magazine</a></li>
                  <li><a href="#">DC Kids</a></li>
                  <li><a href="#">DC Universe</a></li>
                  <li><a href="#">DC Power Visa</a></li>
                </ul>
              </div>
              <!-- /.col-3 -->
            </div>
            <!-- /.row -->
          </div>
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
  .content {
    background-color: $dark;
    height: 100px;
  }

  .banner {
    background-color: $accenture;
    nav {
      height: 100%;
      a {
        font-family: "Bahnschrift SemiBold";
        font-size: 0.9rem !important;
        color: $light !important;
        position: relative;
      }
    }
  }
}

footer {
  .footer_up {
    padding-top: 2rem;
    background-image: url("./assets/img/footer-bg.jpg");
    background-size: cover;
    height: 400px;
    color: $light;

    h2 {
      font-family: "Bahnschrift SemiBold";
      font-size: 1.5rem !important;
    }

    ul {
      padding: 0;
      li {
        list-style: none;
        a {
          text-decoration: none;
          color: $secondary;
          font-size: 0.8rem;
        }
      }
    }

    img {
      position: relative;
      bottom: 15%;
    }
  }

  .footer_down {
    background-color: $darkless;
    height: 100px;
    position: relative;
    z-index: 1;
  }
}
</style>
