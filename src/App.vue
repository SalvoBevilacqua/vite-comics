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
  <div class="header">
    <AppHeader />
  </div>

  <div class="main">
    <AppMain />
  </div>

  <div class="blu">
    <AppBlueSection />
  </div>

  <div class="footer">
    <AppFooter />
  </div>
</template>

<style lang="scss">
@use "./style/general.scss";
</style>
