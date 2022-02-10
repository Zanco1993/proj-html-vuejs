<template>
  <div id="app">
    <header-app />
    <certification-app />
    <service-app />
    <logistic-app />
    <results-app />
    <feedback />
    <get-in-touch />
    <footer-app />
  </div>
</template>

<script>
import HeaderApp from "./components/HeaderApp.vue";
import CertificationApp from "./components/CertificationApp.vue";
import ServiceApp from "./components/ServiceApp.vue";
import LogisticApp from "./components/LogisticApp.vue";
import ResultsApp from "./components/ResultsApp.vue";
import Feedback from "./components/Feedback.vue";
import GetInTouch from "./components/GetInTouch.vue";
import FooterApp from "./components/FooterApp.vue";

export default {
  name: "App",
  components: {
    HeaderApp,
    CertificationApp,
    ServiceApp,
    LogisticApp,
    ResultsApp,
    Feedback,
    GetInTouch,
    FooterApp,
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
@import "./style/variablesColor.scss";
@import "~@fortawesome/fontawesome-free/css/all.css";
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;900&display=swap");
</style>
