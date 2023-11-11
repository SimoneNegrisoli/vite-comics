<template>
  <footer>
    <!-- top -->
    <div class="top">
      <div class="container text-center">
        <div class="row justify-content-between pt-5 pb-5">
          <div class="col-12 col-md-2 d-flex align-items-center justify-content-center felx-nowrap "
            v-for="(el, index) in  footerOpt " :key="index">
            <div class="mydiv">
              <img :src="`/buy-${el.nameImg}`" :alt="el.optTitle" class="mytop-img">
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
      <div class="mylogo-c">
        <img src="../../assets/immagini/dc-logo-bg.png" alt="logo" class="mylogo">
      </div>
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
        </div>
      </div>
    </div>
    <!-- bottom -->
    <div class="bottom pt-4 pb-4">
      <div class="container">
        <div class="row justify-content-between align-items-center">
          <div class="col-12 col-md-4">
            <button class="btn btn-outline-primary ">SIGN-UP NOW</button>
          </div>
          <div class="col-12 col-md-8 d-flex align-items-center align-content-center  justify-content-end ">

            <h5 class="mx-3"><strong>FOLLOW US</strong></h5>
            <div>
              <img src="../../assets/immagini/footer-facebook.png" alt="face">
            </div>
            <div class="mx-3">
              <img src="../../assets/immagini/footer-twitter.png" alt="twitter">
            </div>
            <div>
              <img src="../../assets/immagini/footer-youtube.png" alt="youtube">
            </div>
            <div class="mx-3">
              <img src="../../assets/immagini/footer-periscope.png" alt="periscope">
            </div>
            <div>
              <img src="../../assets/immagini/footer-pinterest.png" alt="pinterest">
            </div>

          </div>
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
          nameImg: 'comics-digital-comics.png'
        },
        {
          optTitle: 'dc merchandise',
          nameImg: 'comics-merchandise.png'
        },
        {
          optTitle: 'subscription',
          nameImg: 'comics-subscriptions.png'
        },
        {
          optTitle: 'dcomic shop locator',
          nameImg: 'comics-shop-locator.png'
        },
        {
          optTitle: 'dc power visa',
          nameImg: 'dc-power-visa.svg'
        }
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
  width: 100%;
}

.top {
  background-color: rgb(56, 128, 241);
  color: white;
  z-index: 100;

  div {
    font-size: 0.8rem;
    white-space: nowrap;
  }
}


.mytop-img {
  height: 40px;
  width: auto;
}

.center {
  background-image: url('../../assets/immagini/footer-bg.jpg');
  color: white;
  position: relative;
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.mylogo-c {
  position: relative;

}

.mylogo {
  width: 500px;
  height: 500px;
  background-size: cover;
  background-repeat: no-repeat;
  position: absolute;
  top: -100px;
  right: 100px;
}

.bottom {
  background-color: rgb(48, 48, 48);
  z-index: 100;

  button {
    color: white;
  }

  img {
    width: 30px;
  }

  h5 {
    color: rgb(56, 123, 234);
    margin-bottom: 0;
  }
}
</style>
