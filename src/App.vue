<template>
  <div id="app">
      <header-app/>
      <main-app/>
      <footer-app/>
  </div>
</template>

<script>
import HeaderApp from "./components/HeaderApp.vue"
import MainApp from "./components/MainApp.vue"
import FooterApp from "./components/FooterApp.vue"

export default {
  name: 'App',
  components: {
    HeaderApp,
    MainApp,
    FooterApp
  }
}
</script>

<style lang="scss">
  @import "./style/general.scss";
  @import "./style/vars.scss";  

  #app {
    position: relative;
    background-color: $bg-purple;
    min-width: 1500px;
  }
</style>
