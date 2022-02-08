<template>
  <div id="app">
    <header-app />
    <main-app />
  </div>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue'
import MainApp from './components/MainApp.vue'
export default {
  name: 'App',
  components: {
    HeaderApp,
    MainApp

  }
}
</script>

<style lang="scss">
@import './style/main.scss';
@import './style/variablesColor.scss';
@import '~@fortawesome/fontawesome-free/css/all.css';
</style>
