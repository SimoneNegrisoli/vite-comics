<template>
  <div class="jumbotron">
    <div class="container">
      <button type="button" class="btn btn-primary fw-bold ">CURRENT SERIES</button>
    </div>
  </div>
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

.jumbotron {
  width: 100%;
  height: 400px;
  background-image: url("../../assets/immagini/jumbotron.jpg");

  button {
    position: relative;
    top: 370px;
    right: 0;
    font-size: 1.4rem;

    :hover {
      font-size: 1.5rem;
    }
  }
}
</style>
