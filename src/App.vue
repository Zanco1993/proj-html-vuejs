<template>
  <div id="app">
    <header-app />
    <certification-app />
  </div>
</template>

<script>
import HeaderApp from "./components/HeaderApp.vue";

import CertificationApp from "./components/CertificationApp.vue";
export default {
  name: "App",
  components: {
    HeaderApp,
    CertificationApp,
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
@import "./style/variablesColor.scss";
@import "~@fortawesome/fontawesome-free/css/all.css";
</style>
