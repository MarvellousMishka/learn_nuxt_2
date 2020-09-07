<template>
  <div>
    <Navigation />
    <nuxt />
    <Footer />
  </div>
</template>
<script>
import Navigation from "~/components/Navigation";
import Footer from "~/components/Footer";
export default {
  components: {
    Navigation,
    Footer,
  },
}
</script>
<style lang="SCSS">
@import '~assets/scss/bootstrap-variables.scss';
@import '~bootstrap/scss/bootstrap.scss';
@import '~bootstrap-vue/src/index.scss';
body {
  padding-top: 100px;
  padding-bottom: 100px;
}
#header-logo {
  max-height: 2rem;
  margin-right: 1.5rem;
}
.nuxt-link-exact-active {
  color: $primary !important;
}
.page-enter-active,
.page-leave-active {
  transition: opacity 0.5s;
}
.page-enter,
.page-leave-to {
  opacity: 0;
}
</style> 