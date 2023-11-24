<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooterUp from "./components/AppFooterUp.vue";
import AppBlueSection from "./components/AppBlueSection.vue";
import AppFooterDw from "./components/AppFooterDw.vue";

export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueSection,
    AppFooterUp,
    AppFooterDw
  }
}
</script>

<template>
  <div class="header">
    <AppHeader />
  </div>

  <div class="jumbo"></div>

  <div class="main">
    <AppMain />
  </div>

  <div class="blu">
    <AppBlueSection />
  </div>

  <div class="footer">
    <div class="up">
      <AppFooterUp />
    </div>

    <div class="down">
      <AppFooterDw />
    </div>
  </div>
</template>

<style lang="scss">
@use "./style/general.scss";
</style>
