<template>
  
    <container>
        <div style="overflow: hidden; position: relative;text-align: center;">
      <div class="slider-swiper">
        <!-- Additional required wrapper -->
        <div class="swiper-wrapper">
          <!-- Slides -->
          <div class="swiper-slide" style="align-items: center;"><img :src="slide1" alt=""></div>
          <div class="swiper-slide" style="align-items: center;"><img :src="slide2" alt=""></div>
          <div class="swiper-slide" style="align-items: center;"><img :src="slide3" alt=""></div>
       
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
    </container>
</template>

<script>
import Swiper from 'swiper/swiper-bundle'
import 'swiper/swiper-bundle.css';

export default {

    data(){
      return{
        slide1 : "imgs/skin1.png",
        slide2 : "imgs/skin2.png",
        slide3 : "imgs/skin3.png"
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