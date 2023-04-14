<script>
export default {
  name: 'SiteHeader',
  data() {
    return {
      menu: [
        {
          text: 'CHARACTERS',
          href: '#'
        },
        {
          text: 'COMICS',
          href: '#'
        },
        {
          text: 'MOVIES',
          href: '#'
        },
        {
          text: 'TV',
          href: '#'
        },
        {
          text: 'GAMES',
          href: '#'
        },
        {
          text: 'COLLECTIBLES',
          href: '#'
        },
        {
          text: 'VIDEOS',
          href: '#'
        },
        {
          text: 'FANS',
          href: '#'
        },
        {
          text: 'NEWS',
          href: '#'
        },
        {
          text: 'SHOP',
          href: '#'
        },
      ],
    }
  }
}
</script>

<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="col-4 d-flex align-items-center">
          <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <!-- /col-4 -->
        <div class="col-8 d-flex align-items-center">
          <ul class="d-flex gap-4">
            <li v-for="item in menu">
              <a :href="item.href">{{ item.text }}</a>
            </li>
          </ul>
        </div>
        <!-- /col-8 -->
      </div>
      <!-- /row -->
    </div>
    <!-- /container -->
  </header>
  <!-- /header -->
</template>


<style lang="scss" scoped>
/* #region Header */
header {
  display: flex;
  align-items: center;
  padding: 1rem 0;
  background-color: white;

  img {
    height: 80px;
  }

  ul {
    list-style: none;
    margin: 0;
    flex-wrap: wrap;

    a {
      text-decoration: none;
      color: black;

      &:hover {
        color: #0282f9;
      }
    }
  }
}

/* #endregion Header */
</style>