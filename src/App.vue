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
  <SiteMain />
  <SiteFooter />
</template>

<style lang="scss">
/* #region Utilities */
ul {
  list-style: none;
}

/* #endregion Utilities */
</style>
