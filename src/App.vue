<template>
  <div id="app">
    <header-app />
    <certification-app />
    <service-app />
  </div>
</template>

<script>
import HeaderApp from "./components/HeaderApp.vue";
import CertificationApp from "./components/CertificationApp.vue";
import ServiceApp from './components/ServiceApp.vue'
export default {
  name: "App",
  components: {
    HeaderApp,
    CertificationApp,
    ServiceApp
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
@import "./style/variablesColor.scss";
@import "~@fortawesome/fontawesome-free/css/all.css";
</style>
