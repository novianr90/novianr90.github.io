<template>
  <div id="app">
    <HeaderSection />
    <AboutSection />
    <PortfolioSection />
    <ContactSection />
  </div>
</template>

<script>
import HeaderSection from './components/HeaderSection.vue'
import AboutSection from './components/AboutSection.vue'
import PortfolioSection from './components/PortfolioSection.vue'
import ContactSection from './components/ContactSection.vue'

export default {
  components: {
    HeaderSection,
    AboutSection,
    PortfolioSection,
    ContactSection
  }
}
</script>

<style>
body {
  font-family: 'Roboto', sans-serif;
  margin: 0;
  padding: 0;
}
#app {
  text-align: center;
}
</style>
