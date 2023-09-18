<template>
  <div id="app">
    <the-header />
    <app-slider />
  </div>
</template>

<script>
import AppSlider from "./components/app-slider.vue";
import theHeader from "./navigation/the-header.vue";
export default {
  components: { theHeader, AppSlider },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #2c3e50;
  width: 100%;
}
</style>
