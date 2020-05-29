<template>
  <div id="app">
    <router-view></router-view>
    <main-bar></main-bar>
  </div>
</template>
<script>
import MainBar from "components/tabbar/MainBar";
export default {
  data() {
    return {};
  },
  components: {
    MainBar
  }
};
</script>

<style lang="scss">
@import "assets/css/base.css";
</style>
