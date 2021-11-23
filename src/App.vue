<template>
  <div id="app">

    <Header />

    <Main />

    <Footer />

    <FooterSubscribe />

  </div>
</template>

<script>
import Header from "@/components/header.vue"
import Main from "@/components/main.vue"
import Footer from "@/components/footer.vue"
import FooterSubscribe from "@/components/footerSubscribe.vue"

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    FooterSubscribe,
  }
}
</script>

<style lang="scss">
@import '@/styles/globals';
@import '@/styles/utilities';
</style>
