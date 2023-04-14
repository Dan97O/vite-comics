<script>
import SiteHeader from "./components/SiteHeader.vue"
import SiteMain from "./components/SiteMain.vue"
import SiteFooter from "./components/SiteFooter.vue"

export default {
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter,
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
  <SiteFooter />
  <!-- /SiteFooter -->
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
</style>
