<template>
  <div id="app">
    <app-navbar />
    <router-view />
  </div>
</template>

<script>
import AppNavbar from "@/components/AppNavbar";

export default {
  components: { AppNavbar }
};
</script>

<style lang="scss">
#app {
  font-family: "Montserrat", Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #4c4c4c;
}
</style>
