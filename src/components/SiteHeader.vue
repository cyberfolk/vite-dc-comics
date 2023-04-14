<script>
export default {
  name: "SiteHeader",
  components: {},
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
            <li class="nav-item active">
              <a class="nav-link" href="#">CHARACTERS</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">COMICS</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">MOVIES</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">TV</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">GAMES</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">COLLECTIBLES</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">VIDEOS</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">FANS</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">NEWS</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">SHOP</a>
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
