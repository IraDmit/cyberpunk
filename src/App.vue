<template>
  <div id="app">
    <the-header />
    <app-slider />
    <app-introduce />
    <app-cta />
    <app-advertisement />
    <app-buy />
    <the-footer />
  </div>
</template>

<script>
import AppAdvertisement from "./components/app-advertisement.vue";
import AppBuy from "./components/app-buy.vue";
import AppCta from "./components/app-cta.vue";
import AppIntroduce from "./components/app-introduce.vue";
import AppSlider from "./components/app-slider.vue";
import TheFooter from "./navigation/the-footer.vue";
import theHeader from "./navigation/the-header.vue";
export default {
  components: {
    theHeader,
    AppSlider,
    AppIntroduce,
    AppCta,
    AppAdvertisement,
    AppBuy,
    TheFooter,
  },
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
