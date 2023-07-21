<template lang="pug">
v-app
  home-navigation
  v-main
    router-view
  home-footer
</template>

<script>
// Components
import HomeNavigation from "@/components/HomeNavigation.vue";
import HomeFooter from "@/components/HomeFooter.vue";

export default {
  name: "App",

  data: () => ({}),
  components: { HomeNavigation, HomeFooter },
};
</script>

<style>
@media screen and (min-width: 1512px) {
  .v-container {
    max-width: 1440px !important;
  }
}
</style>
