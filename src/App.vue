<script>
export default {
  data() {
    return {
      message: "prova",
    };
  },
};

</script>









<template>
  <header class="my-3">
    <div class="container">
      <div class="row">
        <div class="col-4 d-flex align-items-center">
          <img class="img-fluid" src="./assets/img/dc-logo.png" alt="">
        </div>
        <div class="col-8 d-flex align-items-center">
          <ul class="d-flex gap-4">
            <li>
              <a href="#">CHARACTERS</a>
            </li>
            <li>
              <a href="#">COMICS</a>
            </li>
            <li>
              <a href="#">MOVIES</a>
            </li>
            <li>
              <a href="#">TV</a>
            </li>
            <li>
              <a href="#">GAMES</a>
            </li>
            <li>
              <a href="#">COLLECTIBLES</a>
            </li>
            <li>
              <a href="#">VIDEOS</a>
            </li>
            <li>
              <a href="#">FANS</a>
            </li>
            <li>
              <a href="#">NEWS</a>
            </li>
            <li>
              <a href="#">SHOP</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
  <!-- /header -->

  <main>

  </main>
  <!-- /main -->


  <footer>

  </footer>
  <!-- /footer -->
</template>












<style lang="scss">
header {
  height: 100px;
  background-color: white;

  ul {
    list-style: none;

    a {
      text-decoration: none;
      color: black;

      &:hover {
        color: blue;
      }
    }
  }
}
</style>
