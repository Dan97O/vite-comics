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
    <div class="banner_top">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <h3>Content goes here</h3>
          </div>
        </div>
      </div>
    </div>
    <div class="banner_center">
      <div class="container">
        <div class="row">
          <div class="col-12 d-flex justify-content-around">
            <ul>
              <li>
                <a href="#">
                  <img src="./assets/img/buy-comics-digital-comics.png" alt="digital comics">
                  <span>DIGITAL COMICS</span>
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="./assets/img/buy-comics-merchandise.png" alt="merchandise">
                  <span>DC MERCHANDISE</span>
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="./assets/img/buy-comics-subscriptions.png" alt="subscriptions">
                  <span>SUBSCRIPTION</span>
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="./assets/img/buy-comics-shop-locator.png" alt="shop locator">
                  <span>COMIC SHOP LOCATOR</span>
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="./assets/img/buy-dc-power-visa.svg" alt="power-visa">
                  <span>DC POWER VISA</span>
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>

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


main {
  height: calc(100vh - 232px);
  background-color: yellow;

  .banner_top {
    height: 100px;
    background-color: black;
    display: flex;
    align-items: center;
    color: white;
  }

  .banner_center {
    height: 125px;
    background-color: blue;
    display: flex;
    align-items: center;

    ul {
      list-style: none;
      display: flex;
      gap: 4rem;
      margin: 0;

      a {
        text-decoration: none;
        color: black;

        img {
          height: 50px;
        }

        span {
          margin-left: 10px;
          color: white;
        }
      }
    }
  }
}

footer {
  height: 100px;
  background-color: greenyellow;
}
</style>
