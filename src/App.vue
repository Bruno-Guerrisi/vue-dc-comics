<template>
  <div id="app">

    <Header />

    <main>
      
      <MainJumbotron />
      
      <Main />
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
import Footer from "@/components/footer.vue"
import FooterSubscribe from "@/components/footerSubscribe.vue"

export default {
  name: 'App',
  components: {
    Header,
    Main,
    MainJumbotron,
    Footer,
    FooterSubscribe,
  }
}
</script>

<style lang="scss">
@import '@/styles/globals';
@import '@/styles/utilities';
</style>
