<template>
  <div id="app">
    <HeaderComics />
    <MainCont />
    <PageMerch />
    <FooterLinks />
    <FooterSocials />
  </div>
</template>

<script>
import HeaderComics from './components/HeaderComics.vue'
import MainCont from './components/MainCont.vue'
import PageMerch from './components/PageMerch.vue'
import FooterLinks from './components/FooterLinks.vue'
import FooterSocials from './components/FooterSocials.vue'

export default {
  name: 'App',
  components: {
    HeaderComics,
    MainCont,
    PageMerch,
    FooterLinks,
    FooterSocials
  }
}
</script>

<style lang="scss">
@import url(./assets/styles/style.scss);
</style>
