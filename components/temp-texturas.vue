<template>
    <section class="tt">
        <container>
            <div class="ttc">
                <h1>Texturas</h1>
            </div>
        </container>

        <br><br>

        <!-- <container class="cards">
            <div class="swiper"> -->
            <!-- Additional required wrapper -->
            <!-- <div class="swiper-wrapper"> -->
                <!-- Slides -->
                <!-- <div class="swiper-slide">Slide 1</div>
                <div class="swiper-slide">Slide 2</div>
                <div class="swiper-slide">Slide 3</div>
                ... -->
            <!-- </div> -->
            <!-- If we need pagination -->
            <!-- <div class="swiper-pagination"></div> -->

            <!-- If we need navigation buttons -->
            <!-- <div class="swiper-button-prev"></div>
            <div class="swiper-button-next"></div> -->

            <!-- If we need scrollbar -->
            <!-- <div class="swiper-scrollbar"></div>
            </div>
        </container> -->

        <container class="cards">
            <div class="card-deck">
                <div class="card">
                    <img src="../imgs/textura1.jpeg" class="card-img-top" alt="" href="#">
                    <div class="card-body">
                        <h5 class="card-title">
                            <a href="#" target="_blank" class="links">LB Photo Realism Texture Pack</a>
                        </h5>
                        <p class="card-text">
                            Version: 1.19.2 <br>
                            Categories: <a href="#" target="_blank" class="cat">Realista</a> <a href="#" target="_blank" class="cat">Pesada</a> <a href="#" target="_blank" class="cat">Detalhada</a>
                        </p>
                    </div>
                </div>
                <div class="card">
                    <img src="../imgs/textura2.jpeg" class="card-img-top" alt="">
                    <div class="card-body">
                        <h5 class="card-title">
                            <a href="#" target="_blank" class="links">Synthwave PvP Texture Pack</a>
                        </h5>
                        <p class="card-text">
                            Version: 1.19.2 <br>
                            Categories: <a href="#" target="_blank" class="cat">PvP</a> <a href="#" target="_blank" class="cat">+FPS</a> <a href="#" target="_blank" class="cat">Simples</a> <a href="#" target="_blank" class="cat">Leve</a>
                        </p>
                    </div>
                </div>
                <div class="card">
                    <img src="../imgs/textura3.jpeg" class="card-img-top" alt="">
                    <div class="card-body">
                        <h5 class="card-title">
                            <a href="#" target="_blank" class="links">Modern Craft Texture Pack</a>
                        </h5>
                        <p class="card-text">
                            Version: 1.19.2 <br>
                            Categories: <a href="#" target="_blank" class="cat">Construção</a> <a href="#" target="_blank" class="cat">Decoração</a> <a href="#" target="_blank" class="cat">Moderna</a> <a href="#" target="_blank" class="cat">Detalhada</a>
                        </p>
                    </div>
                </div>
            </div>
        </container>
    </section>
</template>

<style lang="scss" scoped >

    .tt{
        padding: 120px 60px;
    }
    .ttc{
        padding: 35px;

        color: white;
        background-color: rgb(127, 158, 177);
        text-align: center;

        h1{
            font-size: 65px;
            font-family: 'VT323', monospace;
        }
    }

    .card{
        border-color: rgb(230, 230, 230);
    }

    .links{
        text-decoration: none;
        color: black;
    }

    .cat{
        text-decoration: none;
        color: black;
        background-color: rgb(205, 205, 205);
        padding: 5px;
        border-radius: 15px;
        font-size: 13px;
    }
</style>
<!-- 
<script>

  export default {
  
    setup() {
      const onSwiper = (swiper) => {
        console.log(swiper);
      };
      const onSlideChange = () => {
        console.log('slide change');
      };
      return {
        onSwiper,
        onSlideChange,
      };
    },
  };
</script> -->