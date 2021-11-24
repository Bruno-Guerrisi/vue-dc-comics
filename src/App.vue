<template>
  <div id="app">

    <Header />

    <main>
      
      <MainJumbotron />

      <Main />

      <MainBonus />
    </main>

    <footer>

      <Footer />

      <FooterSubscribe />
    </footer>

  </div>
</template>

<script>
import Header from "@/components/header.vue"
import Main from "@/components/main.vue"
import MainJumbotron from "@/components/mainJumbotron.vue"
import MainBonus from "@/components/mainBonus.vue"
import Footer from "@/components/footer.vue"
import FooterSubscribe from "@/components/footerSubscribe.vue"

export default {
  name: 'App',
  components: {
    Header,
    Main,
    MainJumbotron,
    MainBonus,
    Footer,
    FooterSubscribe,
  }
}
</script>

<style lang="scss">
@import '@/styles/globals';
</style>
