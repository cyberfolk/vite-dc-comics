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
      <div class="d-flex justify-content-between">
        <img class="my-3" src="./assets/img/dc-logo.png" alt="dc-log" />
        <!-- logo -->
        <nav class="nav">
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
        <!-- /.d-flex -->
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
        <nav class="nav d-flex justify-content-around">
          <a class="nav-link" href="#">
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
          <a class="nav-link d-flex" href="#">
            <img class="py-2" src="./assets/img/buy-dc-power-visa.svg" alt="" />
            <div class="align-self-center">DC POWER VISA</div>
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
          <div class="col-6">
            <button>SIGN-UP NOW!</button>
          </div>
          <!-- /.col-6 -->
          <div class="col-6">
            <div class="d-flex align-items-center h-100 gap-4">
              <div class="follow fs-5">FOLLOW US</div>
              <ul class="list-inline d-flex gap-3 m-0">
                <li>
                  <a href="#"><img src="./assets/img/footer-facebook.png" alt="" /></a>
                </li>
                <li>
                  <a href="#"><img src="./assets/img/footer-twitter.png" alt="" /></a>
                </li>
                <li>
                  <a href="#"><img src="./assets/img/footer-youtube.png" alt="" /></a>
                </li>
                <li>
                  <a href="#"><img src="./assets/img/footer-pinterest.png" alt="" /></a>
                </li>
                <li>
                  <a href="#"><img src="./assets/img/footer-periscope.png" alt="" /></a>
                </li>
              </ul>
            </div>
          </div>
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
  img {
    height: 80px;
  }
  a {
    font-family: "Bahnschrift SemiBold";
    font-size: 0.9rem !important;
    color: $dark !important;
    position: relative;
    line-height: 7; // use the number without units, because I say the total height of the line is 6 font size
  }

  .active {
    color: $accenture !important;
  }

  .active:after {
    content: "";
    position: absolute;
    right: 0;
    bottom: 0;
    height: 6px;
    width: 100%;
    background-color: $accenture;
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
      a {
        font-family: "Bahnschrift SemiBold";
        font-size: 0.9rem !important;
        color: $light !important;
        position: relative;
        img {
          margin: 2rem 0;
          height: 60px;
          padding-right: 1rem;
        }
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
    position: relative;
    z-index: 1;
    padding: 1.8rem 0;

    button {
      border: 2px solid $accenture;
      background-color: transparent;
      color: $light;
      padding: 0.8rem;
      font-weight: 500;
    }
    .follow {
      font-weight: 500;
      color: $accenture;
      align-self: center;
    }
  }
}
</style>
