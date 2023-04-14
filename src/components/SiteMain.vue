<script>
export default {
  name: 'SiteMain',
  data() {
    return {
      banner: [
        {
          text: 'DIGITAL COMICS',
          src: 'buy-comics-digital-comics.png'
        },
        {
          text: 'DC MERCHANDISE',
          src: 'buy-comics-merchandise.png'
        },
        {
          text: 'SUBSCRIPTION',
          src: 'buy-comics-subscriptions.png'
        },
        {
          text: 'COMIC SHOP LOCATOR',
          src: 'buy-comics-shop-locator.png'
        },
        {
          text: 'DC POWER VISA',
          src: 'buy-dc-power-visa.svg'
        },
      ],
    }
  },
  methods: {
    getUrlImg(name) {
      return new URL(`../assets/img/${name}`, import.meta.url).href
    }
  }

}
</script>



<template>
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
              <li v-for="item in banner">
                <a href="#">
                  <img :src="getUrlImg(item.src)" alt="digital comics">
                  <span>{{ item.text }}</span>
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="banner_bottom">
      <div class="container">
        <div class="row">
          <div class="col-6">
            <div class="row">
              <div class="col-4">
                <ul class="pt-4">
                  <li>
                    <a href="#">
                      <h4>
                        DC COMICS
                      </h4>
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Characters
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Comics
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Movies
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      TV
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Games
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Videos
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      News
                    </a>
                  </li>
                </ul>
                <ul>
                  <li>
                    <a href="#">
                      <h4>
                        SHOP
                      </h4>
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Shop DC
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Shop DC Collectibles
                    </a>
                  </li>
                </ul>
              </div>
              <!-- /col-4 -->
              <div class="col-4">
                <ul class="pt-4">
                  <li>
                    <a href="#">
                      <h4>
                        DC
                      </h4>
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Terms Of Use
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Privacy policy (New)
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Ad Choices
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Advertising
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Jobs
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Subscriptions
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Talent Workshops
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      CPSC Certificates
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Ratings
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Shop Help
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      Contacts Us
                    </a>
                  </li>
                </ul>
              </div>
              <!-- /col-4 -->
              <div class="col-4">
                <ul class="pt-4">
                  <li>
                    <a href="#">
                      <h4>
                        SITES
                      </h4>
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      DC
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      MAD Megazine
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      DC Kids
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      DC Universe
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      DC Power Visa
                    </a>
                  </li>
                </ul>
              </div>
              <!-- /col-4 -->
            </div>
            <!-- /row -->
          </div>
          <!-- /col-6 -->
          <div class="logo_dc col-6">
          </div>
          <!-- /logo_dc col-6 -->
        </div>
        <!-- /row -->
      </div>
      <!-- /container -->
    </div>
    <!-- /banner_bottom -->
  </main>
  <!-- /main -->
</template>


<style lang="scss" scoped>
/* #region Main */

main {

  background-color: yellow;

  .banner_top {
    padding: 2rem 0;
    background-color: #1c1c1c;
    display: flex;
    align-items: center;
    color: white;
  }

  .banner_center {
    padding: 2rem 0;
    background-color: #0282f9;
    display: flex;
    align-items: center;
    position: relative;
    z-index: 500;

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

  .banner_bottom {
    background-image: url(../assets/img/footer-bg.jpg);

    ul {
      list-style: none;
      padding: 0;

      li {
        line-height: 18px;

        a {
          text-decoration: none;
          color: rgb(165, 165, 165);
          font-size: 12px;

          &:hover {
            color: rgb(232, 232, 240);
          }

          h4 {
            color: white;
          }
        }
      }
    }

    .logo_dc {
      background-image: url(../assets/img/dc-logo-bg.png);
      height: 500px;
      background-repeat: no-repeat;
      margin-top: -7rem;
      z-index: 0;
    }
  }
}

/* #endregion Main */
</style>