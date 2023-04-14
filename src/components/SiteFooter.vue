<script>
export default {
  name: 'SiteFooter',
  data() {
    return {

    }
  },
}
</script>

<template>
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
              <img src="../assets/img/footer-facebook.png" alt="">
            </li>
            <li>
              <img src="../assets/img/footer-twitter.png" alt="">
            </li>
            <li>
              <img src="../assets/img/footer-youtube.png" alt="">
            </li>
            <li>
              <img src="../assets/img/footer-pinterest.png" alt="">
            </li>
            <li>
              <img src="../assets/img/footer-periscope.png" alt="">
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

<style lang="scss" scoped>
/* #region Footer */
footer {
  padding: 1.5rem 0;
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