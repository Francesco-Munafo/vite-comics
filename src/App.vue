<script>
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
import AppServices from './components/AppServices.vue'
import AppFooterTop from './components/AppFooterTop.vue'
export default {
  data() {

    return {

    }
  },
  components: {
    AppHeader,
    AppJumbo,
    AppServices,
    AppFooterTop
  }
}

</script>

<template>

  <AppHeader></AppHeader>

  <main id="app_main" class="position-relative z-3">

     <AppJumbo></AppJumbo>

  <AppServices></AppServices>

  </main>

  <AppFooterTop></AppFooterTop>

</template>

<style lang="scss">
@use './assets/scss/app.scss';
</style>
