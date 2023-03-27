<script>
import AppBuy from "./components/AppBuy.vue";
import AppNav from "./components/AppNav.vue";
import AppMain from "./components/AppMain.vue";
import AppProps from "./components/AppProps.vue";
export default {
  data() {
    return {
      
    };
  },

  components: {
    AppNav,
    AppMain,
    AppProps,
    AppBuy,
  },
};
</script>

<template>
  <AppNav></AppNav>
  <AppMain></AppMain>
  <AppBuy></AppBuy>
</template>

<style scoped>
</style>
