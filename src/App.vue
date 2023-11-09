<template>
  <div class="header">
    <HeaderApp />
  </div>
  <div class="main">
    <MainContApp />
  </div>
  <div class="footer">
    <FooterApp />
  </div>
</template>

<script>
import HeaderApp from "./components/Header/HeaderApp.vue";
import MainContApp from "./components/Main/MainContApp.vue";
import FooterApp from "./components/Footer/FooterApp.vue";
export default {
  name: "App",
  components: {
    HeaderApp,
    MainContApp,
    FooterApp,
  },
};
</script>

<style lang="scss" scoped></style>
