<template>
  <div id="app">
    <header-app />
    <certification-app />
    <service-app />
    <logistical-app />
  </div>
</template>

<script>
import HeaderApp from "./components/HeaderApp.vue";
import CertificationApp from "./components/CertificationApp.vue";
import ServiceApp from './components/ServiceApp.vue';
import LogisticalApp from './components/LogisticalApp.vue';
export default {
  name: "App",
  components: {
    HeaderApp,
    CertificationApp,
    ServiceApp,
    LogisticalApp
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
@import "./style/variablesColor.scss";
@import "~@fortawesome/fontawesome-free/css/all.css";
</style>
