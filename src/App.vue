<template>
  <headerSite></headerSite>
  <mainSite></mainSite>
  <footerSite></footerSite>
</template>

<script>
import headerSite from './components/header/header.vue'
import mainSite from './components/main/main.vue'
import footerSite from './components/footer/footer.vue'

export default {
  name: 'App',
  components: {
    headerSite,
    mainSite,
    footerSite,
  }
}
</script>

<style>

@font-face {
    font-family: "Roboto";
    src:url('~@/assets/fonts/Roboto-Medium.woff2') format('woff2');
  }
  
  /* @font-face {
    font-family: "Roboto-Bold";
    font-style: bold;
    src:url('~@/assets/fonts/Roboto-Bold.woff2') format('woff2');
  } */
</style>
