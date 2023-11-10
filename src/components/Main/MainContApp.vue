<template>
  <main class="p-5">
    <div class="container">
      <div class="row">
        <div class="col-12 col-md-2" v-for="(comic, index) in comics">
          <CardComp :imgCh="comic.thumb" :titleCh="comic.series" />
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import DcComics from "./dc-comics.js";
import CardComp from './CardComp.vue';
export default {
  name: "MainContApp",
  components: {
    CardComp,
  },
  data() {
    return {
      comics: DcComics
    }
  }

};
</script>

<style lang="scss" scoped>
main {
  color: white;
  background-color: black;
}
</style>
