<template>
  <footer>
    <!-- top -->
    <div class="top">
      <div class="container text-center">
        <div class="row">
          <div class="col-12 col-md-2" v-for="(el, index) in  footerOpt " :key="index">
            <div>
              <img :src="`/buy-comics-${el.nameImg}`" alt="">

            </div>
            <div>

            </div>
          </div>

        </div>
      </div>
    </div>
    <!-- center -->
    <div class="center">
      <div class="container">
        <div class="row">
          <div class="col-12">ciao</div>
        </div>
      </div>
    </div>
    <!-- bottom -->
    <div class="bottom">
      <div class="container">
        <div class="row">
          <div class="col-12">ciao</div>
        </div>
      </div>
    </div>


  </footer>
</template>

<script>
export default {
  name: "FooterApp",
  data() {
    return {
      footerOpt: [
        {
          optTitle: 'digital comics',
          nameImg: 'digital-comics.png'
        },
        {
          optTitle: 'dc merchandise',
          nameImg: 'merchandise.png'
        },
        {
          optTitle: 'subscription',
          nameImg: 'subscriptions.png'
        },
        {
          optTitle: 'dcomic shop locator',
          nameImg: 'shop-locator.png'
        },
        {
          optTitle: 'dc power visa',
          nameImg: 'dc-power-visa.svg'
        },
      ]
    }
  }

};
</script>

<style lang="scss" scoped>
.top {
  background-color: rgb(56, 128, 241);
  color: white;
}

.center {
  background-image: url('../../assets/immagini/footer-bg.jpg');
}

.bottom {
  background-color: rgb(48, 48, 48);
}
</style>
