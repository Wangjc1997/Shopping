<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <router-view />
    <FooterGuide v-show="$route.meta.showFooter" />
  </div>
</template>

<script>
import FooterGuide from "./components/FooterGuide/FooterGuide.vue";
export default {
  name: "App",
  components: {
    FooterGuide,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100%;
  height: 100%;
  background: #f5f5f5;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
