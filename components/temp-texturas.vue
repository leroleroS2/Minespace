<template>
    <section class="tt">
        <container>
            <a href="#" target="_blank" class="ttc2">
                <div class="ttc">
                <h1>Texturas</h1>
                <h5>Clique para ver mais</h5>
            </div>
            </a>
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

        <container>
            <h1>- Mais populares : </h1><br>
        </container>

        <container class="cards">
            <div class="card-deck">
                <div class="card">
                    <a href="#" target="_blank" style="text-decoration: none; color: black;"><img src="../imgs/textura1.jpeg" class="card-img-top" alt="" href="#"></a>
                    <div class="card-body">
                        <h5 class="card-title">
                            <a href="#" target="_blank" class="links">LB Photo Realism Texture Pack</a>
                        </h5>
                        <p class="card-text">
                            Version: 1.19.2 <br>
                            Categorias: <a href="#" target="_blank" class="cat">Textura</a> <a href="#" target="_blank" class="cat">Realista</a> <a href="#" target="_blank" class="cat">Pesada</a> <a href="#" target="_blank" class="cat">Detalhada</a>
                        </p>
                    </div>
                </div>
                <div class="card">
                    <a href="#" target="_blank" style="text-decoration: none; color: black;"><img src="../imgs/textura2.jpeg" class="card-img-top" alt=""></a>
                    <div class="card-body">
                        <h5 class="card-title">
                            <a href="#" target="_blank" class="links">Synthwave PvP Texture Pack</a>
                        </h5>
                        <p class="card-text">
                            Version: 1.19.2 <br>
                            Categorias: <a href="#" target="_blank" class="cat">Textura</a> <a href="#" target="_blank" class="cat">PvP</a> <a href="#" target="_blank" class="cat">+FPS</a> <a href="#" target="_blank" class="cat">Simples</a> <a href="#" target="_blank" class="cat">Leve</a>
                        </p>
                    </div>
                </div>
                <div class="card">
                    <a href="#" target="_blank" style="text-decoration: none; color: black;"><img src="../imgs/textura3.jpeg" class="card-img-top" alt=""></a>
                    <div class="card-body">
                        <h5 class="card-title">
                            <a href="#" target="_blank" class="links">Modern Craft Texture Pack</a>
                        </h5>
                        <p class="card-text">
                            Version: 1.19.2 <br>
                            Categorias: <a href="#" target="_blank" class="cat">Textura</a>  <a href="#" target="_blank" class="cat">Construção</a> <a href="#" target="_blank" class="cat">Decoração</a> <a href="#" target="_blank" class="cat">Moderna</a> <a href="#" target="_blank" class="cat">Detalhada</a>
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

        h1{
            font-family: 'VT323', monospace;
        }
    }
    .ttc{
        padding: 35px;

        color: white;
        background: url(../imgs/fundo-titulo-textura.png);
        text-align: center;

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

    .card{
        border-color: rgb(230, 230, 230);

        .card-text{
            max-width: 500px;
            padding-top: 5px;
            line-height: 28px;
        }
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