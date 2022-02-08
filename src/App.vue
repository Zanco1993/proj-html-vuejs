<template>
  <div id="app">
    <header-app/>
  </div>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue'

export default {
  name: 'App',
  components: {
    HeaderApp
  }
}
</script>

<style lang="scss">
@import './style/main.scss';
@import './style/variablesColor.scss';
@import '~@fortawesome/fontawesome-free/css/all.css';
</style>
