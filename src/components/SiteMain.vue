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
      comics: [
        {
          "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ],
    }
  },
  methods: {
    getUrlImg(name) {
      return new URL(`../assets/img/${name}`, import.meta.url).href
    },

  }

}
</script>



<template>
  <main>
    <div class="banner_top">
      <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="">
      </div>
      <div class="container">
        <button class="btn_series btn-outline-primary">CURRENT SERIES</button>
        <div class="row d-flex justify-content-center mt-3">
          <div class="col-10 d-flex flex-wrap justify-content-evenly g-2">
            <div class="my_card me-3" v-for="img in comics">
              <img :src="(img.thumb)" alt="">
              <div class="text"><span>{{ img.series }}</span></div>
            </div>
          </div>
          <div class=" d-flex justify-content-center my-3">
            <button class="btn-outline-primary">LOAD MORE</button>
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

  .banner_top {
    padding: 0 0 1rem 0;
    background-color: #1c1c1c;
    color: white;

    .jumbotron {
      img {
        height: 400px;
        object-fit: cover;
        object-position: top;
        width: 100%;
      }
    }

    .container {
      margin-top: -12px;

      .btn_series {
        margin-left: 110px;
      }

      button {
        width: 160px;
        background-color: #0282f9;
        color: white;
      }

      .my_card {
        height: 200px;
        width: 150px;
        margin-bottom: 3rem;

        img {
          height: 200px;
          width: 100%;
        }

        .text {
          display: flex;

          margin-top: 5px;
          width: 125px;

          span {
            font-size: 10px;
            text-transform: uppercase;
          }
        }

      }
    }

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