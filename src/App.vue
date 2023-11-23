<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppBlueSection from "./components/AppBlueSection.vue";

export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueSection,
    AppFooter
  }
}
</script>

<template>
  <h1>testo su app</h1>
  <AppHeader />
  <AppMain />
  <AppBlueSection />
  <AppFooter />
</template>

<style lang="scss">
@use "./style/general.scss";
</style>
