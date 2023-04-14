<script>
export default {
  name: "SiteHeader",
  components: {},
};
</script>

<template>
  <header class="mt-4 bg-white">
    <div class="container">
      <div class="d-flex justify-content-between">
        <img class="my-3" src="./../assets/img/dc-logo.png" alt="dc-log" />
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
</template>
