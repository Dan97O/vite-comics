<script>
import SiteHeader from "./components/SiteHeader.vue";
import SiteMain from "./components/SiteMain.vue";

export default {
  components: {
    SiteHeader,
    SiteMain,
  },
  data() {
    return {
      message: "prova",
    };
  },
};

</script>

<template>
  <SiteHeader />
  <!-- /SiteHeader -->

  <SiteMain />
  <!-- /SiteMain -->




  <footer>
    <div class="container">
      <div class="row">
        <div class="col-6 d-flex align-items-center">
          <button>SING-UP NOW!</button>
        </div>
        <!-- col-6 -->
        <div class="col-6 d-flex align-items-center justify-content-end">
          <h4>FOLLOW US</h4>
          <ul class="d-flex gap-2">
            <li>
              <img src="./assets/img/footer-facebook.png" alt="">
            </li>
            <li>
              <img src="./assets/img/footer-twitter.png" alt="">
            </li>
            <li>
              <img src="./assets/img/footer-youtube.png" alt="">
            </li>
            <li>
              <img src="./assets/img/footer-pinterest.png" alt="">
            </li>
            <li>
              <img src="./assets/img/footer-periscope.png" alt="">
            </li>
          </ul>
        </div>
        <!-- col-6 -->
      </div>
      <!-- /row -->
    </div>
    <!-- /container -->
  </footer>
  <!-- /footer -->
</template>

<style lang="scss">
/* #region Utilities */
body {
  height: 100vh;
  overflow-y: hidden;
}

ul {
  list-style: none;
}

/* #endregion Utilities */


/* #region Footer */
footer {
  height: 100px;
  background-color: #303030;
  position: relative;
  z-index: 500;
  display: flex;
  align-items: center;

  button {
    padding: 10px;
    background-color: #303030;
    border-color: #0282f9;
    color: white;
  }

  h4 {
    color: #0282f9;
  }
}

/* #endregion Footer */
</style>
