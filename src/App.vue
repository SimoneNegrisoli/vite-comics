<template>
  <HeaderApp />
  <MainContApp />
  <FooterApp />
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
