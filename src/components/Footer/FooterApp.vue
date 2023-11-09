<template>
  <footer>
    <!-- top -->
    <div class="top">
      <div class="container text-center">
        <div class="row justify-content-between pt-5 pb-5">
          <div class="col-12 col-md-2 d-flex align-items-center justify-content-center felx-nowrap"
            v-for="(el, index) in  footerOpt " :key="index">
            <div>
              <img :src="`/buy-comics-${el.nameImg}`" :alt="el.optTitle">
            </div>
            <div class="mx-3 ">
              {{ el.optTitle.toUpperCase() }}
            </div>
          </div>

        </div>
      </div>
    </div>
    <!-- center -->
    <div class="center pt-4">
      <div class="container">
        <div class="row justify-content-between">
          <div class="col-12 col-md-6">
            <div class="container-fluid">
              <div class="row">
                <div class="col-12 col-md-4">
                  <ul>
                    <h4><strong>DC COMICS</strong></h4>
                    <li>Character</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>Tv</li>
                    <li>Games</li>
                    <li>Video</li>
                    <li>News</li>
                  </ul>
                  <ul>
                    <h4><strong>SHOP DC</strong></h4>
                    <li>Shop Dc</li>
                    <li>Shop Dc Collection</li>
                  </ul>
                </div>
                <div class="col-12 col-md-4">
                  <ul>
                    <h4><strong>DC</strong></h4>
                    <li>Character</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>Tv</li>
                    <li>Games</li>
                    <li>Video</li>
                    <li>News</li>
                    <li>News</li>
                    <li>News</li>
                    <li>News</li>
                    <li>News</li>
                  </ul>
                </div>
                <div class="col-12 col-md-4">
                  <ul>
                    <h4><strong>SITES</strong></h4>
                    <li>Character</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>Tv</li>
                    <li>Tv</li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
          <div class="col-12 col-md-6 text-center ">
            <img src="../../assets/immagini/dc-logo-bg.png" alt="">
          </div>
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
        // {
        //   optTitle: 'dc power visa',
        //   nameImg: 'dc-power-visa.svg'
        // },non mi legge l'immagine svg chiedere il perche
      ]
    }
  }

};
</script>

<style lang="scss" scoped>
ul {
  list-style: none;

  li {
    color: rgb(122, 122, 122);
  }
}

img {
  width: 50px;
}

.top {
  background-color: rgb(56, 128, 241);
  color: white;

  div {
    font-size: 0.8rem;
    white-space: nowrap;
  }
}

.center {
  background-image: url('../../assets/immagini/footer-bg.jpg');
  color: white;

  img {
    width: 100%;
    z-index: -1;
  }
}

.bottom {
  background-color: rgb(48, 48, 48);
}
</style>
