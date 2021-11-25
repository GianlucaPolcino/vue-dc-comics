<template>
  <div>
    <Header />
    <Jumbotron />
    <Main />
    <Section />
    <Footer />
  </div>
</template>

<script>

import Header from "./components/Header.vue"
import Jumbotron from "./components/Jumbotron.vue"
import Main from "./components/Main.vue"
import Section from "./components/Section.vue"
import Footer from "./components/Footer.vue"
export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Main,
    Section,
    Footer,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/vars.scss";
  @import "./assets/style/generals.scss";
  @import "./assets/style/utilities.scss";
</style>
