<template>
  <div>
    <header-ow></header-ow>
    <heroes-ow></heroes-ow>
    <maps></maps>
    <teams></teams>
    <footer-ow></footer-ow>
  </div>
</template>

<script>
import Header from "./components/header.vue";
import Heroes from "./components/heroes.vue";
import Maps from "./components/maps.vue";
import Teams from "./components/teams.vue";
import Footer from "./components/footer.vue";
export default {
  components: {
    "header-ow": Header,
    "heroes-ow": Heroes,
    maps: Maps,
    teams: Teams,
    "footer-ow": Footer
  },
  name: "app",
  data() {
    return {};
  }
};
</script>

<style lang="scss">
body {
  background-color: hsl(210, 38%, 93%);
}
</style>
