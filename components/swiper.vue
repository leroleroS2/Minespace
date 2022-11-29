<template>
  <section class="tt">
    <titulo-temp :title="titulo" class="fundotitulo"/>

    <br><br><br>

    <container>
      <div class="fundo">
        <div class="cont-slider">
          <div style="overflow: hidden; position: relative;text-align: center; width: 1000px;">
              <div class="slider-swiper">
              <!-- Additional required wrapper -->
                <div class="swiper-wrapper">
                  <!-- Slides -->
                  <div class="swiper-slide" style="align-items: center;">
                    <nuxt-link to="/aba-skins">
                      <img :src="slide1" alt="">
                      <h1 class="titulo-slider">Skin de Homem Aranha</h1>
                      <br>
                    </nuxt-link>
                  </div>
                  <div class="swiper-slide" style="align-items: center;">
                    <nuxt-link to="/aba-skins">
                      <img :src="slide2" alt="">
                      <h1 class="titulo-slider">Skin BRASILSILSILSILLL</h1>
                      <br>
                    </nuxt-link>
                  </div>
                  <div class="swiper-slide" style="align-items: center;">
                    <nuxt-link to="/aba-skins">
                      <img :src="slide3" alt="">
                      <h1 class="titulo-slider">Skin listradinho</h1>
                      <br>
                    </nuxt-link>
                  </div>
                  <div class="swiper-slide" style="align-items: center;">
                    <nuxt-link to="/aba-skins">
                      <img :src="slide4" alt="">
                      <h1 class="titulo-slider">Skin de Homem Aranha</h1>
                      <br>
                    </nuxt-link>
                  </div>
                  <div class="swiper-slide" style="align-items: center;">
                    <nuxt-link to="/aba-skins">
                      <img :src="slide5" alt="">
                      <h1 class="titulo-slider">Skin BRASILSILSILSILLL</h1>
                      <br>
                    </nuxt-link>
                  </div>
                  <div class="swiper-slide" style="align-items: center;">
                    <nuxt-link to="/aba-skins">
                      <img :src="slide6" alt="">
                      <h1 class="titulo-slider">Skin listradinho</h1>
                      <br>
                    </nuxt-link>
                  </div>
            
                </div>
                <!-- If we need pagination -->
                <div class="swiper-pagination"></div>

                <!-- If we need navigation buttons -->
                <div class="swiper-button-prev" style="color: #808487;"></div>
                <div class="swiper-button-next" style="color: #808487;"></div>

                <!-- If we need scrollbar -->
                <div class="swiper-scrollbar"></div>
              </div>
            </div>
        </div>
      </div>
    </container>
  </section>
</template>

<style lang="scss">
  .fundotitulo .ttc{
    background: linear-gradient(180deg, #7fb19a, #587a6a);
  }
</style>

<style lang="scss" scoped>

  .fundo{
    background-image: linear-gradient(to right, #ffffff, #f8f8f8, #f0f0f0, #e9e9e9, #e2e2e2, #e2e2e2, #e2e2e2, #e2e2e2, #e9e9e9, #f0f0f0, #f8f8f8, #ffffff);
  }
  .cont-slider{
    text-align: -webkit-center;
    // background-color: linear-gradient(180deg #ffffff, #000000, #ffffff);
  }
  .slider-swiper, .swiper-scrollbar, .swiper-pagination {
    width: 1000px;
    margin-bottom: 15px;
  }

  .titulo-slider{
    padding-bottom: 10px;
    font-size: 30px;
    text-decoration: none;
    color: #000000;
  }
  .tt{
      padding: 120px 60px;

      a{
          text-decoration: none;
      }

      h1{
          font-family: 'VT323', monospace;
      }
  }
  .ttc{
      padding: 35px;

      color: white;
      // background: linear-gradient(180deg, #7fb19a, #587a6a);
      text-align: center;

      // url(../imgs/fundo-titulo-textura.png)

      text-decoration: none;

      .ttc::hover{
        text-decoration: none;
      }

      h1{
        font-size: 65px;
        font-family: 'VT323', monospace;
      }

      h5{
        font-size: 28px;
        font-family: 'VT323', monospace;
      }
  }

  .ttc2{
    color: white;
    text-align: center;

    text-decoration: none;

    .ttc::hover{
        text-decoration: none;
    }
  }
</style>

<script>
import Swiper from 'swiper/swiper-bundle'
import 'swiper/swiper-bundle.css';

export default {

    data(){
      return{
        titulo : "Skins",
        subtitulo : "Clique para ver mais",
        slide1 : "imgs/skin1.png",
        slide2 : "imgs/skin2.png",
        slide3 : "imgs/skin3.png",
        slide4 : "imgs/skin4.png",
        slide5 : "imgs/skin5.png",
        slide6 : "imgs/skin6.png"
      }
    },

    components: {
    Swiper,
    // SwiperSlide,
    },
    mounted(){
    this.init()
    },
    methods: {
    init(){
        const swiper = new Swiper('.slider-swiper', {
    // Optional parameters
        // loop: true,
        // If we need pagination
        pagination: {
        el: '.swiper-pagination',
        },

        // Navigation arrows
        navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
        },

        // And if we need scrollbar
        scrollbar: {
        el: '.swiper-scrollbar',
        },
    });
    }
    }
    
};
</script>